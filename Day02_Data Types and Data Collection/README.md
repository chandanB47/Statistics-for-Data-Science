# Day 02 — Data Types and Data Collection

**Level:** Beginner  
**Estimated time:** 60–90 minutes  
**Tools:** Excel or Google Sheets  
**Dataset:** [`../datasets/day02_customer_profiles.csv`](../datasets/day02_customer_profiles.csv)

## Learning Objectives

By the end of this lesson, you should be able to:
- Distinguish categorical and numerical variables.
- Recognize nominal, ordinal, interval, and ratio measurement scales.
- Identify discrete and continuous numerical variables.
- Explain observational and experimental data.
- Recognize common sampling methods and sources of bias.
- Choose summaries that fit the type of variable.

## 1. Why Data Types Matter

Before calculating statistics, identify what each column represents. A variable's type influences which summaries, charts, and statistical methods are meaningful.

For example, calculating an average of customer ages is meaningful. Calculating an average of customer IDs is not: an ID is a label, even if it contains digits.

## 2. Categorical vs. Numerical Data

### Categorical data
Categorical variables place observations into groups or labels.

Examples:
- `Region`: North, South, East, West
- `Subscription_Tier`: Basic, Standard, Premium
- `Satisfaction_Score`: rating from 1 to 5 (treated as ordinal in this lesson)

You can count categories and calculate proportions. Whether arithmetic is meaningful depends on the measurement scale.

### Numerical data
Numerical variables represent counts or measurements.

- **Discrete:** countable values, often whole numbers. Example: number of orders.
- **Continuous:** measurements that can conceptually take values across a range. Example: age or spending, even if recorded to a limited number of decimal places.

| Variable | Broad type | Why |
|---|---|---|
| Region | Categorical | Labels identify groups |
| Number of orders | Numerical, discrete | A count |
| Monthly spend | Numerical, often treated as continuous | A measured amount |
| Customer ID | Identifier / categorical label | Digits do not make it a quantity |

## 3. Four Measurement Scales

### Nominal — names, no natural order
Examples: region, product category, customer ID.
- Group membership is meaningful.
- You can count each category and find the mode.
- A numerical code assigned to a category does not make it quantitative.

### Ordinal — ordered categories
Examples: satisfaction rating (1–5), education level, subscription tier.
- Order is meaningful.
- The distance between levels is not necessarily equal.
- Category proportions and the median may be useful; interpret averages carefully.

### Interval — equal differences, no meaningful absolute zero
Classic example: temperature in Celsius or Fahrenheit.
- Differences are meaningful.
- Ratios are not: 20°C is not “twice as hot” as 10°C.

### Ratio — equal differences and a meaningful zero
Examples: age, monthly spending, number of orders, distance.
- Differences and ratios are meaningful.
- Zero means none of the measured quantity.
- Spending of ₹4,000 is twice ₹2,000.

| Scale | Ordered? | Equal differences? | Meaningful zero? | Example |
|---|---|---|---|---|
| Nominal | No | No | Not applicable | Region |
| Ordinal | Yes | Not guaranteed | Not applicable | Satisfaction level |
| Interval | Yes | Yes | No | Temperature in °C |
| Ratio | Yes | Yes | Yes | Monthly spend |

**Important:** Numbers used as category labels do not automatically make a variable quantitative. A satisfaction score of 1–5 is commonly treated as ordinal unless the analysis justifies another approach.

## 4. Observational vs. Experimental Data

### Observational data
The analyst observes what happens without assigning a treatment.

Example: compare spending by region using existing transaction records.

**Limitation:** Groups may differ in other ways. An observed relationship alone does not establish cause and effect.

### Experimental data
The researcher assigns a treatment or condition, ideally randomly.

Example: randomly assign eligible customers to see either an old offer or a new offer, then compare purchase rates.

Random assignment can help support causal conclusions when the experiment is properly designed and conducted.

## 5. Common Sampling Methods

- **Simple random sampling:** each member has a known, equal chance of selection.
- **Systematic sampling:** select every k-th record after a starting point.
- **Stratified sampling:** divide the population into meaningful groups, then sample from each group.
- **Cluster sampling:** randomly select groups/clusters, then collect data within selected clusters.
- **Convenience sampling:** select people who are easiest to reach; quick but often prone to bias.

### Sampling bias
Sampling bias occurs when the selection process systematically distorts which members are represented.

Example: surveying only customers who visit a store on weekday mornings may miss customers who shop at other times.

A large sample does not automatically remove bias. Nonresponse and measurement errors can also affect results.

## 6. Dataset Guide

Open [`day02_customer_profiles.csv`](../datasets/day02_customer_profiles.csv).

| Column | Description | Expected interpretation |
|---|---|---|
| `Customer_ID` | Fictional identifier | Nominal label; do not average |
| `Region` | Customer region | Nominal categorical |
| `Subscription_Tier` | Basic, Standard, Premium | Ordinal categorical |
| `Satisfaction_Score` | Rating from 1 to 5 | Ordinal in this lesson |
| `Age_Years` | Age in years | Numerical, ratio |
| `Monthly_Spend_INR` | Monthly spending in rupees | Numerical, ratio |
| `Orders_Last_Month` | Count of orders | Numerical, discrete ratio |
| `Signup_Date` | Date customer joined | Date variable; time differences are meaningful |
| `Survey_Response` | Yes/No response | Nominal categorical |

This is a **synthetic practice dataset**, not real customer information.

## 7. Practical Steps in Excel or Google Sheets

1. Open the CSV file.
2. For each column, write its broad type: categorical, numerical, date, or identifier.
3. Identify the measurement scale where appropriate: nominal, ordinal, interval, or ratio.
4. Count customers in each region using a PivotTable or `COUNTIF`.
5. Count the `Yes` and `No` survey responses.
6. Calculate the proportion of `Yes` responses.
7. Notice that `Customer_ID` contains letters and numbers but is still an identifier, not a measurement.
8. Complete [`TASK.md`](TASK.md).

### Helpful spreadsheet formulas

Assuming `Region` is column B, `Survey_Response` is column I, and data rows are 2–31:

- Count customer records: `=COUNTA(A2:A31)`
- Count customers in North: `=COUNTIF(B2:B31,"North")`
- Count Yes responses: `=COUNTIF(I2:I31,"Yes")`
- Proportion of Yes responses: `=COUNTIF(I2:I31,"Yes")/COUNTA(I2:I31)`

Format the last result as a percentage. Adjust references if your columns differ.

## Day 02 Completion Checklist

- [ ] I can distinguish categorical and numerical data.
- [ ] I can explain discrete versus continuous variables.
- [ ] I can identify nominal, ordinal, interval, and ratio scales.
- [ ] I understand observational versus experimental data.
- [ ] I can name common sampling methods and explain sampling bias.
- [ ] I classified the dataset columns and completed `TASK.md`.
