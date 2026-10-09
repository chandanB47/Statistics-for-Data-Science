# Day 01 — Statistics Foundations

**Level:** Beginner  
**Estimated time:** 60–90 minutes  
**Tools:** Excel or Google Sheets (Python is optional today)  
**Dataset:** [`../datasets/day01_customer_spending.csv`](../datasets/day01_customer_spending.csv)

## Today's Goal

Understand the language of statistics and apply it to a small customer dataset. By the end, you should be able to explain:
- What statistics is used for in data analysis.
- Population versus sample.
- Parameter versus statistic.
- Descriptive versus inferential statistics.
- Why sampling methods and data limitations matter.

## 1. What Is Statistics?

**Statistics** is the discipline of collecting, organizing, analyzing, interpreting, and communicating data to answer questions and make decisions under uncertainty.

A business example: a retailer has customer spending records. An analyst summarizes spending, compares groups, and estimates how all customers might behave using a sample.

### Statistics versus tools

| Item | Main purpose |
|---|---|
| SQL / database | Store, retrieve, filter, join, and aggregate data |
| Excel | Organize data and calculate summaries |
| Python | Automate analysis and run statistical methods |
| Power BI | Present findings through reports and dashboards |
| Statistics | Provide methods for summarizing data, quantifying uncertainty, and evaluating evidence |

A tool can calculate an average; statistical thinking helps you decide what the average means and whether it answers the question.

## 2. Population and Sample

- **Population:** the complete group you want to understand.
- **Sample:** a subset selected from that population.

In today's dataset, each row represents one fictional customer from a defined group of 30 customers.
- For this exercise, the **population** is all 30 customers in the file.
- Customers with `Selected_For_Sample = Yes` form the **sample** selected for a short survey exercise.

A sample can save time and money, but the way it is selected matters. A sample is not automatically representative just because it contains several customers.

## 3. Parameter and Statistic

- **Parameter:** a numerical summary describing a population.
- **Statistic:** a numerical summary calculated from a sample.

Example:
- Mean spending of all 30 customers = population parameter for this defined dataset.
- Mean spending of only the selected customers = sample statistic.

In real work, the population parameter is often unknown. Analysts use sample statistics to estimate it and should communicate uncertainty.

Common notation:
- Population mean: \(\mu\) (mu)
- Sample mean: \(\bar{x}\) (x-bar)
- Population standard deviation: \(\sigma\) (sigma)
- Sample standard deviation: \(s\)

You do not need to memorize the symbols today; understand the population/sample distinction first.

## 4. Descriptive versus Inferential Statistics

**Descriptive statistics** summarize the data you have observed.
- Example: “The 30 customers in this file have an average monthly spend of ₹X.”
- Examples of methods: tables, mean, median, percentages, charts.

**Inferential statistics** use sample data to estimate a population value or evaluate a claim about a population.
- Example: “Using the selected customers, estimate average spending for the full customer group.”
- Examples of methods: confidence intervals and hypothesis tests (covered later).

| Descriptive | Inferential |
|---|---|
| Summarizes observed data | Uses sample evidence to draw conclusions about a population |
| Describes the customers in the file | Estimates or tests a claim about a broader target group |
| Does not automatically explain causes | Conclusions depend on sampling, design, and assumptions |

## 5. Dataset Guide

Open `datasets/day01_customer_spending.csv`.

| Column | Meaning |
|---|---|
| `Customer_ID` | Fictional customer identifier |
| `Region` | Customer region |
| `Age` | Customer age in years |
| `Monthly_Spend_INR` | Fictional monthly spend in Indian rupees |
| `Orders_Last_Month` | Number of orders in the previous month |
| `Satisfaction_Score` | Fictional satisfaction score from 1 to 5 |
| `Selected_For_Sample` | Whether the customer is included in the exercise sample |

**Dataset note:** This is a small synthetic practice dataset. It does not represent real people or a real company. The 30 rows are the complete population only for this exercise; do not generalize the results to real customers.

## 6. Worked Example: Mean

Suppose four daily sales amounts are ₹1,000, ₹2,000, ₹1,500, and ₹3,500.

Total:
\[
1{,}000 + 2{,}000 + 1{,}500 + 3{,}500 = ₹8{,}000
\]

Mean:
\[
\bar{x} = \frac{\text{sum of observations}}{\text{number of observations}}
= \frac{8{,}000}{4} = ₹2{,}000
\]

The total answers “How much altogether?” The mean answers “What was the average per recorded day?”

## 7. Practical Steps

1. Download the dataset linked above and open it in Excel or Google Sheets.
2. Count the number of rows/customers.
3. Filter `Selected_For_Sample` to `Yes` and count those rows.
4. Calculate the average `Monthly_Spend_INR` for all customers.
5. Calculate the average `Monthly_Spend_INR` for selected sample customers only.
6. Compare the two averages. They may differ; that alone does not prove the sample is bad.
7. Complete each question in [`TASK.md`](TASK.md).
8. Save your answers or screenshots, then send them for review before moving to Day 02.

### Helpful spreadsheet formulas

Assuming `Monthly_Spend_INR` is column D and `Selected_For_Sample` is column G, with headers in row 1 and data in rows 2–31:

- Count customer records: `=COUNTA(A2:A31)`
- Population mean for this file: `=AVERAGE(D2:D31)`
- Count selected sample: `=COUNTIF(G2:G31,"Yes")`
- Sample mean: `=AVERAGEIF(G2:G31,"Yes",D2:D31)`

If your columns differ, adjust the cell references.

## Day 01 Completion Checklist

- [ ] I can explain what statistics is used for.
- [ ] I can identify the population and sample.
- [ ] I can distinguish a parameter from a statistic.
- [ ] I can distinguish descriptive from inferential statistics.
- [ ] I opened and analyzed the dataset.
- [ ] I completed `TASK.md` and submitted my answers for review.
