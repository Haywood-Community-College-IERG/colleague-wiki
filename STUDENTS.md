<!-- TOC -->

- [STUDENTS](#students)
    - [Field: STU.TYPES](#field-stutypes)
    - [Special college specific definitions](#special-college-specific-definitions)
        - [Haywood CC](#haywood-cc)

<!-- /TOC -->

# STUDENTS

## Field: STU.TYPES 
 
| Code | Description                | Notes  |
| ---- | -------------------------- | ------ |
| CCPP | Career and College Promise | \*HCC  |
 
## Special college specific definitions

### Haywood CC
<details>
<summary>Special definitions for Haywood Community College</summary>

\* This can be used to identify CCP and EC students. Must
   use ACAD.PROGRAMS and INSTITUTIONS.ATTEND as follows:

* If student is in a CCP or EC program, then assign then accordingly
* If student is not in a CCP or EC program but does have a STU.TYPES == 'CCPP', 
  then assign them as follows:
    * if student is active in the early college (INSTA.INSTITUTIONS.ID == '1113888'),
      then assign as EC
    * If student is NOT active in the early college, then assign as CCP
* If student is not in CCP or EC program nor do they have a STU.TYPE == 'CCPP' then 
  assign them as Non-CCP.
</details>

