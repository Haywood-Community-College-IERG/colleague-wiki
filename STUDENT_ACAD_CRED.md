<!-- TOC -->

- [STUDENT_ACAD_CRED](#student_acad_cred)
    - [Dictionary](#dictionary)
    - [Fields: STC.VERIFIED.GRADE, STC.FINAL.GRADE](#fields-stcverifiedgrade-stcfinalgrade)
    - [Field: STC.STATUS](#field-stcstatus)
    - [Special college specific definitions](#special-college-specific-definitions)
        - [Field: STC.SECTION.NO](#field-stcsectionno)

<!-- tocstop -->
# STUDENT_ACAD_CRED

### Dictionary


### Fields: STC.VERIFIED.GRADE, STC.FINAL.GRADE 

| Code | Description | Notes                     | Grade Scheme |
| ---- | ----------- | ------------------------- | ------------ |
| 25   | U           | Unsatisfactory            | BSP          |
| 26   | W           | Withdrawn                 | BSP          |
| 27   | W           | Withdrawal                | CU           |
| 28   | CT          | Continue                  | CU           |
| 29   | TR          | Transfer Credit           | CU           |
| 30   | TP          | Tech Prep Credit          | CU           |
| 31   | AP          | Advanced Placement Credit | CU           |
| 32   | CE          | Credit by Exam            | CU           |
| 33   | P           | Pass                      | CE           |
| 35   | P           | Pass                      | BSP          |
| 36   | NS          | No Show                   | CU           |
| 37   | WF          | Withdrawal Failing        | CU           |
| 38   | NG          | Not Graded                | CU           |
| 39   | NS          | No Show                   | CE           |
| 40   | D           | Drop                      | CE           |
| 41   | CT          | Continuation              | BSP          |
| 43   | DP          | Developmental Pass        | CU           |
| 44   | EP          | Evaluation Pass           | HSGPA        |
| 45   | EN          | Evaluation Not Pass       | HSGPA        |
| 47   | SR          | Senior Audit              | CU           |
| 48   | EL          | Experiential Learning     | CU           |
| 51   | I           | Incomplete                | CE           |
| 52   | \*F         | \*F                       | CU           |
| 1    | A           | Excellent                 | CU           |
| 2    | B           | Above Average             | CU           |
| 3    | C           | Average                   | CU           |
| 4    | D           | Below Average             | CU           |
| 6    | F           | Failing                   | CU           |
| 7    | I           | Incomplete                | CU           |
| 8    | P           | Pass                      | CU           |
| NC   | DR          | Developmental Repeat      | CU           |
| 9    | AU          | Audit                     | CU           |
| 14   | F           | Failing                   | CE           |
| 15   | S           | Satisfactory              | CE           |
| 16   | U           | Unsatisfactory            | CE           |
| 17   | W           | Withdrawn                 | CE           |
| 18   | AU          | Audit                     | CE           |
| 19   | A           | Excellent                 | BSP          |
| 20   | B           | Above Average             | BSP          |
| 21   | C           | Average                   | BSP          |
| 22   | D           | Below Average             | BSP          |
| 23   | F           | Failing                   | BSP          |
| 24   | S           | Satisfactory              | BSP          |


### Field: STC.STATUS 
 
| Code | Description             | Notes                                                               |
| ---- | ----------------------- | ------------------------------------------------------------------- |
| N    | New                     | (1)                                                                 |
| A    | Add                     | (2)                                                                 |
| W    | Withdrawn               | (4) Class is dropped after census or 10% mark                       |
| C    | Cancelled               | (6) Class is cancelled                                              |
| NS   | No Show                 | (3)                                                                 |
| NP   | Non-Payment             | (5)                                                                 |
| X    | Deleted                 | (5) Class is dropped before start date                              |
| D    | Dropped                 | (3) Class is dropped after start date but before census or 10% mark |
| TR   | Transfer Equiv Eval     | (7)                                                                 |
| NC   | Noncourse Equivalency   | (7)                                                                 |
| XT   | External Transfer Equiv | (7)                                                                 |
| PR   | Preliminary Equiv Eval  | (0)                                                                 |
 

### Special college specific definitions

<details>
<summary>Special definitions for Haywood Community College</summary>

#### Field: STC.SECTION.NO

| Pattern | Examples      | Location        | Short-semester | Hybrid | High School           | Course Type       | Web-based | Night |
|---------|---------------|-----------------|----------------|--------|-----------------------|-------------------|-----------|-------|
| 0#      | 01 - 09       | Campus          |                |        |                       |                   |           |       |
| 6#      | 61 - 66       | Campus          |                |        |                       | Lab               |           |       |
| 9#      | 99            | Campus          |                |        |                       | Independent Study |           |       |
| A#      | A1 - A3       | Campus          | TRUE           |        |                       |                   |           |       |
| A6#     | A60 - A66     | Campus          | TRUE           |        |                       | Lab               |           |       |
| C0#     | C01           | Central Haywood |                |        | Central Haywood       |                   |           |       |
| C6#     | C60           | Central Haywood |                |        | Central Haywood       | Lab               |           |       |
| CA#     | CA1           | Central Haywood | TRUE           |        | Central Haywood       |                   |           |       |
| EM##    | EM01 - EM99   | Math Emporium   |                |        |                       |                   |           |       |
| EMY##   | EMY01 - EMY99 | Math Emporium   |                | TRUE   |                       |                   |           |       |
| H0#     | H01 - H03     | Campus          |                |        | Haywood Early College |                   |           |       |
| HW#     | HW1           | Online          |                |        | Haywood Early College |                   | TRUE      |       |
| IH##    | IH01 - IH99   | Information Hwy |                |        |                       |                   |           |       |
| IN#     | IN1 - IN2     | Internet        |                |        |                       |                   |           |       |
| INA#    | INA1 - INA3   | Internet        | TRUE           |        |                       |                   |           |       |
| J##     | J01 - J99     | JobsNow         |                |        |                       |                   |           |       |
| K##     | K01 - K99     | Cherokee        |                |        | Cherokee?             |                   |           |       |
| N#      | N1 - N2       | Campus          |                |        |                       |                   |           | TRUE  |
| N6#     | N60 - N61     | Campus          |                |        |                       | Lab               |           | TRUE  |
| NA#     | NA1 - NA2     | Campus          | TRUE           |        |                       |                   |           | TRUE  |
| NS#     | NS1 - NS2     | Self-Supporting |                |        |                       |                   |           | TRUE  |
| NW#     | NW1           | Online          |                |        |                       |                   | TRUE      | TRUE  |
| NWA#    | NWA1          | Online          | TRUE           |        |                       |                   | TRUE      | TRUE  |
| P0#     | P01 - P02     | Pisgah          |                |        | Pisgah                |                   |           |       |
| PA#     | PA1 - PA2     | Pisgah          | TRUE           |        | Pisgah                |                   |           |       |
| PY#     | PY1 - PY2     | Pisgah          |                | TRUE   | Pisgah                |                   |           |       |
| S#      | S1 - S2       | Self-Supporting |                |        |                       |                   |           |       |
| T0#     | T01           | Campus          |                |        | Tuscola               |                   |           |       |
| T6#     | T60           | Campus          |                |        | Tuscola               | Lab               |           |       |
| TA#     | TA1           | Campus          | TRUE           |        | Tuscola               |                   |           |       |
| TW#     | TW1           | Online          |                |        | Tuscola               |                   | TRUE      |       |
| TWA#    | TWA1          | Online          | TRUE           |        | Tuscola               |                   | TRUE      |       |
| TY#     | TY1           | Campus          |                | TRUE   | Tuscola               |                   |           |       |
| WB      | WB            | Campus          |                |        |                       |                   |           |       |
| W#      | W1 - W3       | Online          |                |        |                       |                   | TRUE      |       |
| WA#     | WA1 - WA2     | Online          | TRUE           |        |                       |                   | TRUE      |       |
| Y#      | Y1            | Campus          |                | TRUE   |                       |                   |           |       |

</details>

