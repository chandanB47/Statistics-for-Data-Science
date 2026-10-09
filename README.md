# Statistics-for-Data-Science



A structured, practical journey from **statistics fundamentals to applied statistical analysis** for Data Analyst and entry-level Data Science work. This repository uses a day-by-day learning format with concepts, worked examples, separate tasks, and a final portfolio project.

> **Learning principle:** Understand what a method tells you, when it is appropriate, what assumptions it makes, and how to explain its result. Do not memorize formulas without understanding their meaning.

## Objectives

By the end of this challenge, I aim to:
- Describe datasets using tables, visualizations, and summary statistics.
- Understand probability, random variables, and common distributions.
- Measure variability and investigate outliers.
- Interpret correlation and regression while distinguishing association from causation.
- Understand sampling, sampling variability, standard errors, and confidence intervals.
- Perform and interpret basic hypothesis tests.
- Select statistical methods based on the business question and data types.
- Communicate conclusions, uncertainty, limitations, and recommendations.
- Complete a reproducible, portfolio-ready statistical analysis.

## 15-Day Roadmap: Basics to Applied/Advanced Topics

| Day | Topic | Key skills | Practical deliverable |
|---|---|---|---|
| 01 | Foundations of Statistics | Statistics vs. data storage, population/sample, parameter/statistic, descriptive/inferential statistics | Foundation exercises |
| 02 | Data Types and Data Collection | Categorical/numerical data, measurement scales, observational vs. experimental data, sampling methods, bias | Data classification worksheet |
| 03 | Frequency Tables and Visualization | Counts, proportions, percentages, bar charts, histograms, box plots | Frequency table and charts |
| 04 | Central Tendency | Mean, median, mode, weighted mean; choosing robust summaries | Summary calculations |
| 05 | Variability and Outliers | Range, variance, standard deviation, quartiles, percentiles, IQR, z-scores | Variability and outlier analysis |
| 06 | Descriptive Statistics Project | Missing data checks, grouped summaries, distribution interpretation, clear reporting | Small dataset analysis |
| 07 | Probability Fundamentals | Events, complements, addition/multiplication rules, independence, conditional probability | Probability exercises |
| 08 | Random Variables and Distributions | Discrete/continuous variables, expected value, variance, binomial and normal distributions, z-scores | Distribution problems and plots |
| 09 | Relationships Between Variables | Covariance, Pearson correlation, rank correlation, scatter plots, correlation limitations | Relationship analysis |
| 10 | Sampling and Sampling Distributions | Sampling bias, sampling variability, Central Limit Theorem, standard error | Sampling simulation or worksheet |
| 11 | Estimation and Confidence Intervals | Point estimates, confidence levels, interval interpretation, sample-size intuition | Confidence interval exercise |
| 12 | Hypothesis Testing | Null/alternative hypotheses, test statistics, p-values, significance, Type I/II errors, power basics | Written test interpretation |
| 13 | Statistical Tests and A/B Testing | t-tests, paired vs. independent samples, chi-square tests, practical vs. statistical significance | Test-selection case study |
| 14 | Regression and Causal Reasoning | Simple linear regression, coefficients, residuals, R², assumptions, confounding, correlation vs. causation | Regression interpretation |
| 15 | End-to-End Portfolio Project | Formulate question, clean data, explore, select methods, interpret uncertainty, report recommendations | Reproducible analysis and final report |

**Scope note:** Fifteen days is an intensive introduction. “Advanced” here means applying core methods thoughtfully, understanding assumptions, and interpreting results—not mastery of every advanced statistical theory.

## Repository Structure

```text
Statistics-for-Data-Science/
├── README.md
├── progress-tracker.md
├── .gitignore
├── datasets/
│   └── README.md
└── Day-01/
    ├── README.md
    └── TASK.md
```

Add `Day-02/` through `Day-15/` as each day is prepared. Day-specific notebooks, datasets, charts, and reports should be added only when useful.

## Daily Learning Workflow

1. Read the day's `README.md`.
2. Review definitions, notation, assumptions, formulas, and worked examples.
3. Complete the day's separate `TASK.md`.
4. Check calculations and explain the result in plain language.
5. Share answers or screenshots for review before advancing.
6. Update `progress-tracker.md`.
7. Commit completed work to GitHub.

**Suggested time:** 60–120 minutes per day. Allow extra time for probability, confidence intervals, and hypothesis testing if these are new.

## Tools

- **Excel:** formulas, summaries, frequency tables, and quick validation.
- **SQL:** filtering, grouping, aggregation, and preparing analysis-ready data.
- **Python:** reproducible calculations and statistical tests when they add value.
- **Power BI:** communicating descriptive findings through reports and dashboards.

Useful Python libraries:
- `pandas` — data manipulation and summaries
- `numpy` — numerical calculations and random sampling
- `scipy.stats` — probability distributions and statistical tests
- `matplotlib` / `seaborn` — statistical visualizations
- `statsmodels` — statistical models and regression summaries

Not every topic needs Python. First understand the concept, then use the simplest suitable tool.

## Final Portfolio Project

The final project will investigate one clear business question using a suitable dataset. It should include:

1. Business question and intended decision.
2. Dataset source, field descriptions, row count, and limitations.
3. Data-quality checks: missing values, duplicates, invalid values, and relevant assumptions.
4. Descriptive statistics and appropriate visualizations.
5. Relationship analysis or group comparisons, if relevant.
6. A justified confidence interval, hypothesis test, or regression only when suitable.
7. Interpretation in business language.
8. Limitations, uncertainty, possible bias, and confounding.
9. Evidence-based recommendations.
10. Reproducible analysis and a concise final report.

Do not apply every test automatically. Choose a method based on the question, variable types, study design, and assumptions. A statistically significant result does not necessarily imply a large or important business effect; correlation alone does not establish causation.

## Progress

See [`progress-tracker.md`](progress-tracker.md) for daily completion status.

## Learning Checklist

For every method, be able to answer:
- **What is it?**
- **When should I use it?**
- **What assumptions does it require?**
- **How do I interpret the result?**
- **What can it not tell me?**

## Key Takeaway

Statistics is a framework for reasoning under uncertainty. The goal is not merely to calculate a number; it is to select an appropriate method, interpret evidence carefully, and communicate a defensible conclusion.
