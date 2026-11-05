# Methodology

## 1. Business Problem

Identify which factors influence student performance and which students are at risk, so schools can target support.

## 2. Data Source

| Item | Detail |
|---|---|
| Source | student_performance_dataset.csv |
| Records | 1,000 students |
| Format | CSV |

## 3. Data Preparation (Power Query)

| Step | Action |
|---|---|
| 1 | Imported the source file |
| 2 | Checked and set data types |
| 3 | Checked for nulls and duplicates |
| 4 | Renamed columns for clarity |
| 5 | Loaded to the data model |

## 4. Data Model

A single `Students` table with a separate `Measure` table for DAX measures. 

## 5. Dashboard Design

| Page | Purpose | Visuals |
|---|---|---|
| Overview | Headline performance | 5 KPI cards, column chart of final grade distribution |
| Dashboard Drivers | What drives scores | Scatter plots with trend lines: study time, previous grades, attendance vs final score |
| Demographics & Access | Equity lens | Average score by parental education and by internet access |

**Design choices**

| Choice | Reason |
|---|---|
| KPI cards at the top of every page | Constant context while exploring |
| Page-navigation buttons | Simple, app-like navigation |
| Gender and Internet Access slicers | Let users segment the whole report |
| Scatter plots with trend lines | Show direction and strength of relationships at a glance |
| Single blue palette | Clean, consistent look |

## 6. Validation

KPI values were cross-checked against the grade distribution chart (see `dax_measures.md`).

## 7. Limitations

- Correlation does not imply causation.
- Averages can hide individual variation.
- Small differences (e.g. parental education) may be noise.
- No statistical significance tests were run.
