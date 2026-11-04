# Data Dictionary

**Table:** `Students`  
**Rows:** 1,000 (one row per student)

> Column names below are my best reading of the dashboard. Match them to the Data view in Power BI.

| Column | Type | Description | Example |
|---|---|---|---|
| StudentID | Text | Unique student identifier | REPLACE |
| Gender | Text | Female / Male | Female |
| InternetAccess | Text | Whether the student has internet access: Yes / No | Yes |
| ParentalEducation | Text | Highest parental education: None, High School, Bachelors, Masters, PhD | Masters |
| StudyTime | Decimal | Average study time (REPLACE unit, e.g. hours per day) | REPLACE |
| Attendance | Decimal | Attendance rate (REPLACE: percentage) | REPLACE |
| PreviousGrade | Decimal | Previous grade, scale 0–100 | REPLACE |
| FinalScore | Decimal | Final exam score, scale 0–100 | REPLACE |
| FinalGrade | Text | Letter grade: A, B, C, D, F | B |

## Grade Distribution

| Grade | Students | Share |
|---|---|---|
| A | 284 | 28.4% |
| B | 354 | 35.4% |
| C | 261 | 26.1% |
| D | 89 | 8.9% |
| F | 12 | 1.2% |
| **Total** | **1,000** | **100%** |

## Derived Categories

| Category | Definition |
|---|---|
| Pass | FinalGrade is not F |
| At Risk | FinalGrade is D or F |
| Top Performer | FinalGrade is A |
