# Which Factors Are Associated with Student Performance?

An exploratory data analysis (EDA) of exam scores from 1,000 students. This project investigates whether gender, parental education, lunch type, and test preparation are associated with academic performance.

## Links

- [Interactive Dashboard](https://haiderimran019.github.io/student-performance-analysis/student_performance_dashboard.html)
- [GitHub Repository](https://github.com/haiderimran019/student-performance-analysis)

## Project Overview

This project analyzes student performance in mathematics, reading, and writing. It uses Python, pandas, NumPy, matplotlib, seaborn, and SciPy to explore score distributions, relationships between subjects, and differences between student groups.

The analysis is exploratory and focuses on associations in the dataset. It does not establish causal relationships.

## Research Questions

This project examines:

- Are mathematics, reading, and writing scores related?
- Is test preparation associated with average academic performance?
- Is parental education associated with student scores?
- Is lunch type associated with average performance?
- Are there differences in performance by gender?
- How are student scores distributed across subjects?

## Dataset

The project uses the **Students Performance in Exams** dataset.

- [Dataset source on Kaggle](https://www.kaggle.com/datasets/spscientist/students-performance-in-exams)
- Number of records: 1,000 students
- Number of columns: 8
- Main variables: gender, race/ethnicity, parental education, lunch type, test preparation, mathematics score, reading score, and writing score

Please check the original dataset page for its current terms, attribution requirements, and redistribution permissions before sharing the raw CSV publicly.

## Files

| File | Description |
|---|---|
| `student_performance_analysis.ipynb` | Full EDA notebook with data checks, summary statistics, statistical analysis, charts, and limitations |
| `student_performance_dashboard.html` | Interactive dashboard that runs directly in a web browser |
| `StudentsPerformance.csv` | Dataset used in the analysis |
| `chart1_grade_distribution.png` | Grade-band distribution chart |
| `chart2_correlation_heatmap.png` | Subject-score correlation heatmap |
| `chart3_math_vs_reading_scatter.png` | Mathematics versus reading scatterplot |
| `chart4_score_by_test_prep.png` | Average score by test-preparation status |
| `chart5_score_by_parental_education.png` | Average score by parental-education group |
| `score_distributions.png` | Score distributions by subject |

## Methods

The analysis includes:

- Dataset inspection.
- Missing-value checks.
- Duplicate checks.
- Descriptive statistics.
- Average-score calculations.
- Grade-band categorization.
- Correlation analysis.
- Group comparisons.
- Independent-samples t-tests.
- One-way ANOVA.
- Data visualizations.
- Interactive dashboard filtering.

The overall average score is calculated as:

```text
Average score = (math score + reading score + writing score) / 3
