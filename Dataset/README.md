# Shared Dataset

**File:** `customer_campaign_data.csv`

This file contains 300 synthetic customer-level records created for learning. It does not represent real customers or a real company.

| Column | Meaning | Type |
|---|---|---|
| `customer_id` | Unique record ID | Identifier |
| `age` | Age in years | Numerical, discrete |
| `gender` | Category | Categorical, nominal |
| `region` | Broad region | Categorical, nominal |
| `acquisition_channel` | How the customer arrived | Categorical, nominal |
| `campaign_group` | Campaign label A or B | Categorical, nominal |
| `website_visits` | Number of recorded visits | Numerical, discrete |
| `session_minutes` | Session duration | Numerical, continuous |
| `converted` | 1 = converted, 0 = did not convert | Binary categorical |
| `revenue` | Revenue; zero if not converted | Numerical, continuous |
| `satisfaction_score` | Rating from 1 to 5 | Ordinal |
| `support_tickets` | Number of support tickets | Numerical, discrete |

## Notes
- Nine `satisfaction_score` values are missing intentionally for data-quality practice.
- Do not average `customer_id`; it is an identifier.
- The mean of `converted` is the conversion proportion.
- Revenue has many zeros because non-converters have zero revenue.
- Do not claim campaign group differences prove causation. This is a synthetic learning dataset, not a documented randomized experiment.

Open in Excel/Google Sheets. In Python, use `pandas.read_csv("datasets/customer_campaign_data.csv")`.
