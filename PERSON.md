<!-- toc -->

- [PERSON](#PERSON)
    + [Field: PER.RACES](#Field-PERRACES)
    + [Field: PER.ETHNICS](#Field-PERETHNICS)
    + [Field: X.ETHNICS.RACES](#Field-XETHNICSRACES)

<!-- tocstop -->
# PERSON

### Field: PER.RACES 
 
| Code | Description               | Notes  |
| ---- | ------------------------- | ------ |
| AN   | American/Alaska Native    |        |
| AS   | Asian                     |        |
| BL   | Black or African American |        |
| HP   | Hawaiian/Pacific Islander |        |
| WH   | White                     |        |
| NP   | Asian/Pacific Islander    | This should not be used anymore as Pacific Islander has been merged with Hawaiian. |
 

### Field: PER.ETHNICS 

| Code | Description         | Notes |
| ---- | ------------------- | ----- |
| HIS  | Hispanic/Latino     |       |
| NHS  | Non Hispanic/Latino |       |
 

### Field: X.ETHNICS.RACES 
```javascript
string[] xlResult1;  
string[] xlResult2;  
string[] xlResult3;  

key xKeyForeignPerson for file ForeignPerson; 
xKeyForeignPerson = vId;  

if (vFperAlienStatus == "Y") { 
    xKeyForeignPerson = vId; 
    xlResult1 = ("FOR").ToArray((253).Char()); 
} else { 
    if (IsNull((vlPerEthnics).ToDelimitedString((253).Char())) && IsNull((vlPerRaces).ToDelimitedString((253).Char()))) { 
        xlResult1 = ("UNK").ToArray((253).Char()); 
    } else { 
        if ((vlPerEthnics).ToDelimitedString((253).Char()) == "HIS") { 
            xlResult1 = ("HIS").ToArray((253).Char()); 
        } else { 
            if (((vlPerRaces).ToDelimitedString((253).Char())).DCount((253).Char()) > 1) { 
                xlResult1 = ("MULTI").ToArray((253).Char()); 
            } else { 
                xlResult1 = vlPerRaces; 
            } 
        } 
    } 
} 

xlResult2 = xlResult1; 
xlResult3 = xlResult2; 
return xlResult3.ToDelimitedString((253).Char()); 
```