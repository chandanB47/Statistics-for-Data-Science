# Day 02 — Tasks: Data Types and Data Collection

**Estimated time:** 15–25 minutes  
**Dataset:** `../datasets/customer_campaign_data.csv`

Keep answers short and use your own words. There are only 3 tasks.

## Task 1 — Classify the variables
Classify each column as **categorical**, **numerical**, or **identifier**. For numerical variables, also say whether it is discrete or continuous when appropriate.

| Column | Your answer |
|---|---|
| `customer_id` | Identifier |
| `age` | Numerical |
| `region` | Categorical |
| `acquisition_channel` | Categorical |
| `campaign_group` | Categorical |
| `website_visits` | Numerical |
| `session_minutes` | Numerical |
| `converted` | Categorical (binary: 0/1) |
| `revenue` |  Numerical |
| `satisfaction_score` |  Categorical (ordered rating) |
| `support_tickets` |  Numerical |

## Task 2 — Measurement scale
Choose the best scale—**nominal, ordinal, interval, or ratio**—and give one short reason for each:

1. **Region — Nominal:** Regions are categories with no natural ranking.
2. **Satisfaction score — Ordinal:** Scores have a meaningful order, from lower to higher satisfaction, but the differences between scores are not necessarily equal.
3. **Session minutes — Ratio:** Time has a meaningful zero, and a 10-minute session is twice as long as a 5-minute session.

## Task 3 — Collection and bias
Answer in 1–3 sentences each:

### 1. Is this a real experiment or a synthetic learning dataset? Can we conclude that campaign B causes more revenue than campaign A?

The CSV file does not establish whether the data is real or synthetic, so its provenance must be confirmed from the dataset documentation. We cannot conclude that campaign B causes more revenue than campaign A from these records alone because the file does not establish that customers were randomly assigned to campaigns or that other factors were controlled.

### 2. What bias might occur if only customers who bought something were surveyed?

This creates **selection bias** because customers who purchased may have different satisfaction levels from visitors who did not purchase. The survey would not represent all visitors fairly, so the estimated overall satisfaction could be misleading.

## Before you submit
- [x] I classified all listed columns.
- [x] I answered the measurement-scale questions.
- [x] I explained the causation limitation and possible bias.

Next -  moving to Day 03.
