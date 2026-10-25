# Day 02 — Data Types and Data Collection

**Time:** 30–45 minutes  
**Dataset:** `../datasets/customer_campaign_data.csv`

## Goal
Recognize variable types and understand data collection and bias.

## 1. Two main data types
- **Categorical:** labels or groups, such as `region` and `acquisition_channel`.
- **Numerical:** quantities, such as `age`, `website_visits`, and `revenue`.

Numerical variables can be:
- **Discrete:** counts, usually whole numbers, such as `website_visits`.
- **Continuous:** measurements that can take decimal values, such as `session_minutes`.

## 2. Measurement scales
- **Nominal:** categories without a natural order. Example: `region`.
- **Ordinal:** categories with an order. Example: `satisfaction_score` from 1 to 5.
- **Interval:** equal differences are meaningful, but zero is not an absolute absence. Example: temperature in °C.
- **Ratio:** equal differences and a meaningful zero. Example: `revenue` and `session_minutes`.

The storage format does not always define the variable's meaning. `converted` uses 0 and 1 but represents two categories. `customer_id` looks code-like, but is only an identifier.

## 3. How data is collected
- **Observational data:** researchers observe without assigning a treatment.
- **Experimental data:** researchers assign a treatment or condition, ideally at random, then compare outcomes.

Sampling methods:
- **Simple random:** every eligible record has a known, equal chance of selection.
- **Stratified:** split into important groups, then sample within each group.
- **Convenience:** select records that are easiest to reach.

**Sampling bias** occurs when selection makes a sample systematically unrepresentative. A large sample can still be biased.

## Worked example
The mean of `converted` (1 = converted, 0 = not converted) is the proportion of records that converted. The mean of `customer_id` is meaningless because it is only an identifier.

## Quick workflow
1. Open the CSV in Excel or Google Sheets.
2. Inspect the headers and a few rows.
3. Complete `TASK.md`.
4. After complete day02 moving to Day 03.
