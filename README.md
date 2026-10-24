# Statistics for Data Science

A beginner-friendly, 15-day practical journey from statistics fundamentals to applied analysis for Data Analyst and entry-level Data Science work.

**Learning principle:** Understand what a method tells you, when it is appropriate, what assumptions it makes, and how to explain the result. Do not memorize formulas without understanding their meaning.

## Objectives
- Describe data with tables, visualizations, and summary statistics.
- Understand probability and common distributions.
- Measure variability and investigate outliers.
- Interpret correlation and regression without confusing association with causation.
- Understand sampling, standard errors, and confidence intervals.
- Interpret basic hypothesis tests.
- Choose methods based on the business question and data types.
- Communicate uncertainty, limitations, and recommendations.
- Complete a reproducible portfolio project.

## 15-Day Roadmap

| Day | Topic | Simple deliverable |
|---|---|---|
| 01 | Foundations of Statistics | Identify population, sample, parameter, statistic |
| 02 | Data Types and Data Collection | Classify variables and identify possible bias |
| 03 | Frequency Tables and Visualization | One frequency table and one chart |
| 04 | Central Tendency | Mean, median, and mode |
| 05 | Variability and Outliers | Range, IQR, and outlier check |
| 06 | Descriptive Statistics Project | Summary of the shared dataset |
| 07 | Probability Fundamentals | A few probability questions |
| 08 | Random Variables and Distributions | Explore a distribution and expected value |
| 09 | Relationships Between Variables | Scatter plot and correlation interpretation |
| 10 | Sampling and Sampling Distributions | Compare a sample with the full dataset |
| 11 | Estimation and Confidence Intervals | Interpret one confidence interval |
| 12 | Hypothesis Testing | Explain a null hypothesis and p-value |
| 13 | Statistical Tests and A/B Testing | Compare campaign groups appropriately |
| 14 | Regression and Causal Reasoning | Interpret a simple regression and limitations |
| 15 | End-to-End Portfolio Project | Short evidence-based report |

**Scope note:** Fifteen days is an introduction, not mastery of every advanced statistical theory.

## Repository Structure

```text
Statistics-for-Data-Science/
├── README.md
├── progress-tracker.md
├── .gitignore
├── datasets/
│   ├── README.md
│   └── customer_campaign_data.csv
└── Day-02/
    ├── README.md
    └── TASK.md
```

Add each later day's folder as it is prepared.

## Daily Workflow
1. Read the day's `README.md`.
2. Review the short concepts and worked example.
3. Complete `TASK.md` (maximum 3 tasks).
4. Explain results in plain language.
5. Share answers or screenshots for review before advancing.
6. Update `progress-tracker.md`.
7. Commit completed work to GitHub.

**Suggested time:** 30–45 minutes per day.

## Tools
- **Excel / Google Sheets:** formulas, frequency tables, summaries, and charts.
- **SQL:** filtering, grouping, aggregation, and preparing data.
- **Python:** reproducible calculations and statistical tests when useful.
- **Power BI:** communicate descriptive findings in reports and dashboards.

Use the simplest suitable tool. Not every topic needs Python.

## Can One Dataset Be Used for All 15 Days?
Yes. This project uses `datasets/customer_campaign_data.csv` for continuity. It supports most topics, including variable classification, frequency tables, summaries, variability, probability, distributions, sampling, confidence intervals, group comparisons, correlation, and introductory regression.

A single dataset cannot perfectly demonstrate every statistical design. If a topic needs data that this dataset cannot support, we can use a tiny additional example just for that lesson. Campaign group differences in this synthetic dataset do **not** prove causation.

## Final Portfolio Project
Business question: **How do customer engagement and campaign group relate to conversion and revenue?**

The final report should include the business question, dataset and limitations, data-quality checks, descriptive statistics, useful charts, one suitable comparison or relationship analysis, interpretation, and recommendations.

Do not apply every test automatically. Choose methods based on the question, variable types, study design, and assumptions. Statistical significance does not automatically mean a large business effect; correlation alone does not establish causation.

## Progress
See [`progress-tracker.md`](progress-tracker.md).

## Checklist for Every Method
- What is it?
- When should I use it?
- What assumptions does it require?
- How do I interpret the result?
- What can it not tell me?
