# ACAD_CREDENTIALS

## Important Fields

* ACAD.CREDENTIALS.ID - System-generated sequential key to file. [PRIMARY KEY]
* ACAD.PERSON.ID - Single-valued pointer to the PERSON file (since PEOPLE will go away after conversion). [FOREIGN KEY]
* ACAD.ACAD.PROGRAM - Acad Program - This is the academic program in which this academic credential was received.  It is updated by the UACF process in ST and is not meant to be modified by users.  It was needed for the IPEDS Completions Survey, which is a report that needs the CIP code of an academic program for degrees conferred. [FOREIGN KEY]
* ACAD.MAJORS - Majors - Multi-valued pointer to OTHER.MAJORS file.  Displayed but not otherwise used by the system. [FOREIGN KEY]
* ACAD.DEGREE - Degree - Single-valued pointer to OTHER.DEGREES file.  Which specifies a degree earned for an institution attended making up an academic credential. [FOREIGN KEY]
* ACAD.CCD - CCD - Multi-valued pointer to OTHER.CCDS (credential, certificate, diploma) file.  Displayed but not otherwise used by the system. [FOREIGN KEY]
* ACAD.TERM - Term - Term in which ACAD.CREDENTIALS record was created.
* ACAD.TANSCRIPT.ADDRESS - Address - This is the address lines of the graduation transcript address.  AACRAO guidelines stipulated that the first address to which transcripts were sent on graduation be kept for historical purposes.  This is that address. It will be stamped on the ACAD.CREDENTIALS file as well.
* ACAD.TANSCRIPT.CITY - This is the city of the graduation transcript address.  AACRAO guidelines stipulated that the first address to which transcripts were sent on graduation be kept for historical purposes.  This is that address. It will be stamped on the ACAD.CREDENTIALS file as well.
* ACAD.TANSCRIPT.STATE - This is the state/province of the graduation transcript address.  AACRAO guidelines stipulated that the first address to which transcripts were sent on graduation be kept for historical purposes.  This is that address. It will be stamped on the ACAD.CREDENTIALS file as well.
* ACAD.TANSCRIPT.ZIP - This is the zip/postal code of the graduation transcript address.  AACRAO guidelines stipulated that the first address to which transcripts were sent on graduation be kept for historical purposes.  This is that address. It will be stamped on the ACAD.CREDENTIALS file as well.
* ACAD.TANSCRIPT.COUNTRY - This is the country of the graduation transcript address.  AACRAO guidelines stipulated that the first address to which transcripts were sent on graduation be kept for historical purposes.  This is that address. It will be stamped on the ACAD.CREDENTIALS file as well.
* ACAD.INSTITUTIONS.ID - Key to INSTITUTIONS.ATTEND record from ACAD.CREDENTIALS. [FOREIGN KEY]
* ACAD.GPA - Cum GPA - GPA associated with the academic credential.  Displayed, but not otherwise used by the system.
* ACAD.START.DATE - Academic Credential Start Date
* ACAD.END.DATE - Academic Credential End Date
* ACAD.CAST.DATE - Award Date - Created for California MIS reporting. The CAST.SP extract needs a data element to hold either the ACAD.DEGREE.DATE, or the first ACAD.CCD.DATE for use in the list specifications.
* ACAD.CCD.DATE - Certificate Date - Date the CCD (credential, certificate, diploma) was awarded.  (Display varies according to institution parameters.)  Displayed but not otherwise used by the system.
* ACAD.DEGREE.DATE - Degree Date - Date the degree was received.
* ACAD.COMMENCEMENT.DATE - Commencement Date - To store the date that Commencement takes place, Past or Future

### Field: ACAD.CAST.DATE

Returns the ACAD.DEGREE.DATE or the ACAD.CCD.DATE, whichever is not null.
