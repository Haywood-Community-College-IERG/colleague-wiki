<!-- toc -->

- [STUDENT_ACAD_CRED](#STUDENT_ACAD_CRED)
    + [Fields: STC.VERIFIED.GRADE, STC.FINAL.GRADE](#Fields-STCVERIFIEDGRADE-STCFINALGRADE)
    + [Field: STC.STATUS](#Field-STCSTATUS)

<!-- tocstop -->
# STUDENT_ACAD_CRED

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
| C    | Cancelled               | (6) Class is cancelled by HCC                                       |
| NS   | No Show                 | (3)                                                                 |
| NP   | Non-Payment             | (5)                                                                 |
| X    | Deleted                 | (5) Class is dropped before start date                              |
| D    | Dropped                 | (3) Class is dropped after start date but before census or 10% mark |
| TR   | Transfer Equiv Eval     | (7)                                                                 |
| NC   | Noncourse Equivalency   | (7)                                                                 |
| XT   | External Transfer Equiv | (7)                                                                 |
| PR   | Preliminary Equiv Eval  | (0)                                                                 |
 