# Which Factors Are Associated With Student Performance?

An exploratory data analysis (EDA) of 1,000 students' exam scores, looking at
whether gender, parental education, lunch type (socioeconomic proxy), and
test preparation are associated with academic performance.

**Live dashboard:** [Explore the interactive dashboard](https://haiderimran019.github.io/student-performance-analysis/student_performance_dashboard.html)

**Dataset:** [Students Performance in Exams](https://www.kaggle.com/datasets/spscientist/students-performance-in-exams)
— 1,000 rows, 8 columns (gender, race/ethnicity, parental level of education,
lunch, test preparation course, math/reading/writing scores).

## What's in this repo

| File | What it is |
|---|---|
| `student_performance_analysis.ipynb` | Full EDA notebook — missing-value checks, summary stats, grade distributions, correlation analysis, 5 charts, limitations section. Pre-run with all outputs saved. |
| `student_performance_dashboard.html` | Interactive dashboard — filter by gender/race/parental education/lunch/test prep and watch KPIs, charts, and the data table update live. Open directly in any browser, no server needed. |
| `StudentsPerformance.csv` | Raw dataset. |
| `chart*.png`, `score_distributions.png` | Individual chart exports from the notebook. |

## Key findings

- Math, reading, and writing scores are **strongly correlated** with each
  other (r ≈ 0.80–0.95) — students strong in one subject tend to be strong
  across the board.
- **Test preparation**, **parental level of education**, and **lunch type**
  are all statistically significantly associated with average score
  (t-tests / one-way ANOVA, p < 0.001 in each case).
- Gender differences are smaller and subject-dependent (higher reading/writing
  for females, slightly higher math for males), largely netting out on the
  combined average.

## Limitations

**Correlation does not prove causation.** These are observational
associations, not controlled experiments — parental education, lunch type,
and test prep are all entangled with income, school resources, and other
unmeasured factors. See the notebook's Limitations section for the full
discussion.

## How to run it

```bash
pip install pandas numpy matplotlib seaborn scipy jupyter
jupyter notebook student_performance_analysis.ipynb
```

Or just open `student_performance_dashboard.html` in your browser — no
install needed.

## Tools

Python, pandas, NumPy, matplotlib, seaborn, SciPy (statistics).
