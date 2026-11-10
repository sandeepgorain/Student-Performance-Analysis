# STUDENT PERFORMANCE ANALYSIS
### Data Analytics Internship Project

**Project:** Student Performance Analysis  
**Student:** Sandeep Gorain  
**Technology:** Python, Pandas, NumPy, Matplotlib, Seaborn  
**Environment:** Visual Studio Code / Jupyter Notebook  
**Project Type:** Exploratory Data Analysis (EDA)

---

## 1. Executive Summary

This project focuses on analyzing student academic performance using Python and data analytics libraries.

Two datasets were analyzed: Mathematics and Portuguese student performance datasets.

The main objective was to clean and explore the datasets, calculate academic statistics, investigate relationships between different student characteristics and grades, and present meaningful findings through visualizations.

The analysis identified several interesting patterns:

- Portuguese students achieved a higher average final grade than Mathematics students.
- Approximately 67.09% of Mathematics students scored at least 10 out of 20.
- Previous academic failures showed a negative relationship with final grades.
- Previous examination grades showed strong positive correlations with final grades.
- Absence counts showed almost no linear correlation with final grades.

The project demonstrates the complete process of transforming raw datasets into meaningful analytical insights.

## 2. Project Objectives

The main objectives were:

1. Load and understand student performance datasets.
2. Inspect dataset structure and data types.
3. Identify missing values and duplicate records.
4. Perform data cleaning and preparation.
5. Calculate average academic grades.
6. Compare Mathematics and Portuguese performance.
7. Investigate gender-wise academic performance.
8. Analyze study time and student attendance.
9. Identify high-, medium- and low-performing students.
10. Investigate correlations between academic variables.
11. Create meaningful data visualizations.
12. Summarize findings and provide recommendations.

## 3. Dataset Description

Two CSV datasets were used.

| Dataset | Records | Columns |
|---|---:|---:|
| Mathematics | 395 | 33 |
| Portuguese | 649 | 33 |

### Important Features

| Feature | Description |
|---|---|
| school | Student's school |
| sex | Student's gender |
| age | Student's age |
| address | Urban or rural residence |
| famsize | Family size |
| Medu | Mother's education |
| Fedu | Father's education |
| studytime | Weekly study time |
| failures | Previous class failures |
| schoolsup | Extra educational support |
| internet | Internet access |
| absences | Number of school absences |
| G1 | First-period grade |
| G2 | Second-period grade |
| G3 | Final grade |

The grade columns range from 0 to 20.

## 4. Technologies Used

| Technology | Purpose |
|---|---|
| Python | Programming language |
| Pandas | Data manipulation and analysis |
| NumPy | Numerical operations |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| Jupyter Notebook | Interactive analysis |
| VS Code | Development environment |

## 5. Data Cleaning and Preparation

The datasets were loaded using Pandas.

Initial inspection included:

- Dataset dimensions.
- First five records.
- Column information.
- Data types.
- Missing-value detection.
- Duplicate-record detection.
- Numerical and categorical feature identification.

The cleaning checks did not identify missing values or duplicate records in the inspected datasets.

The datasets were then prepared for exploratory analysis.

A separate performance classification was created for Mathematics students:

| Category | Grade Range |
|---|---|
| Low | 0–9 |
| Medium | 10–14 |
| High | 15–20 |

A separate Pass/Fail classification was also created using 10/20 as the project's analytical threshold.

## 6. Exploratory Data Analysis

### 6.1 Subject-wise Performance

| Subject | Students | Average Final Grade |
|---|---:|---:|
| Mathematics | 395 | 10.42 |
| Portuguese | 649 | 11.91 |

Portuguese achieved approximately 1.49 higher average grade points than Mathematics.

### 6.2 Gender-wise Performance

| Gender | Average Mathematics Grade |
|---|---:|
| Female | 9.97 |
| Male | 10.91 |

Male students achieved a higher average Mathematics grade in this sample.

### 6.3 Study Time Analysis

| Study Time Category | Average Final Grade |
|---|---:|
| 1 | 10.05 |
| 2 | 10.17 |
| 3 | 11.40 |
| 4 | 11.26 |

Students in study-time categories 3 and 4 achieved higher average grades than students in categories 1 and 2.

### 6.4 Pass/Fail Analysis

Using 10/20 as the analytical passing threshold:

| Result | Students | Percentage |
|---|---:|---:|
| Pass | 265 | 67.09% |
| Fail | 130 | 32.91% |

Approximately 67% of Mathematics students scored at least 10.

### 6.5 Performance Distribution

| Category | Students | Percentage |
|---|---:|---:|
| Low | 130 | 32.91% |
| Medium | 192 | 48.61% |
| High | 73 | 18.48% |

Medium-performing students represented the largest group.

### 6.6 Previous Failures Analysis

| Previous Failures | Average Final Grade |
|---:|---:|
| 0 | 11.25 |
| 1 | 8.12 |
| 2 | 6.24 |
| 3 | 5.69 |

Students with more previous failures generally achieved lower average Mathematics grades.

### 6.7 Parental Education Analysis

Higher parental education levels generally showed higher average Mathematics grades across education levels 1–4.

However, education level 0 contained very few observations, so its average should be interpreted cautiously.

### 6.8 Absence Analysis

The correlation between absences and final Mathematics grades was approximately 0.034.

This indicates a negligible linear relationship.

## 7. Correlation Analysis

Important correlation results:

| Variables | Correlation |
|---|---:|
| G1 and G2 | 0.852 |
| G1 and G3 | 0.801 |
| G2 and G3 | 0.905 |
| Failures and G3 | -0.360 |
| Studytime and G3 | 0.098 |
| Absences and G3 | 0.034 |

### Important Interpretations

**Previous academic performance:**

G2 showed the strongest positive correlation with G3 (0.905).

**Previous failures:**

Previous failures showed a moderate negative correlation with final grades.

**Study time:**

Study time showed a weak positive linear relationship with final grades.

**Absences:**

Absences showed almost no linear relationship with final grades.

Correlation does not establish causation.

## 8. Data Visualizations

The following visualizations were created:

1. Mathematics Pass/Fail Analysis.
2. Subject-wise Performance Comparison.
3. Gender-wise Academic Performance.
4. Study Time vs Academic Performance.
5. Student Absences vs Final Grades.
6. Student Performance Distribution.
7. Mathematics Grade Distribution.
8. Portuguese Grade Distribution.
9. Academic Performance Correlation Heatmap.
10. Previous Failures vs Academic Performance.
11. Mother's Education vs Student Performance.
12. Father's Education vs Student Performance.

All visualizations were saved in PNG format in the project's visualization directory.

## 9. Key Findings

The major findings of this project are:

1. Portuguese students achieved a higher average final grade than Mathematics students.
2. Approximately one-third of Mathematics students scored below the analytical passing threshold.
3. Medium-performing students represented the largest performance group.
4. Previous examination grades were strongly associated with final grades.
5. Previous academic failures were associated with lower final grades.
6. Study time showed a weak positive relationship with final grades.
7. Absence counts showed almost no linear correlation with final grades.
8. Parental education levels showed generally positive associations with student performance.

## 10. Recommendations

Based on the analysis, the following recommendations could be considered:

- Provide additional academic support to low-performing students.
- Monitor students' examination performance regularly.
- Identify students with previous academic failures for additional guidance.
- Encourage effective study habits.
- Investigate attendance patterns alongside other academic and personal factors.
- Consider students' educational backgrounds when designing academic support programs.

These are suggested interventions based on descriptive findings, not proven causal solutions.

## 11. Limitations

1. The analysis is based on the available datasets and variables.
2. Mathematics and Portuguese datasets contain different numbers of records and were not directly joined for individual-level comparisons.
3. Correlation does not establish causation.
4. Some parental education categories have very small sample sizes.
5. The Pass/Fail threshold of 10/20 was selected for this project and should not be interpreted as a verified official passing rule.
6. The analysis does not establish the effects of all possible socioeconomic and personal factors.

## 12. Conclusion

The Student Performance Analysis project successfully demonstrates the use of Python for data cleaning, exploratory data analysis, statistical investigation and visualization.

Through the analysis of Mathematics and Portuguese datasets, meaningful patterns were identified in academic performance, previous examination results, study time, previous failures, attendance and parental education.

The project helped demonstrate how raw datasets can be transformed into understandable insights that may support better academic decision-making.

It also provided practical experience with Pandas, NumPy, Matplotlib, Seaborn and Jupyter Notebook.

---

**Project Status:** Exploratory Data Analysis and Visualization Completed.

**Developed by:** Sandeep Gorain