# Data Dictionary

**Table:** `Students`  
**Rows:** 1,000 (one row per student)

| Column | Type | Description |
|---|---|---|
| Student ID | Text | Unique student identifier |
| Gender | Text | Female / Male |
| Internet Access | Text | Whether the student has internet access: Yes / No |
| Parental Education | Text | Highest parental education: None, High School, Bachelors, Masters, PhD |
| Study Time | Decimal | Average study time (hours per day) |
| Attendance | Decimal | Attendance rate (percentage, 0–100) |
| Previous Grade | Decimal | Previous grade, scale 0–100 |
| Final Score | Decimal | Final exam score, scale 0–100 |
| Final Grade | Text | Letter grade: A, B, C, D, F |

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
| Pass | Final Grade is not F |
| At Risk | Final Grade is D or F |
| Top Performer | Final Grade is A |
