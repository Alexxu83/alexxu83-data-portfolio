# Retailer Segmentation Using RFM Analysis

## Project Overview

This project applies RFM (Recency, Frequency, Monetary) analysis to retailer transaction data to derive behavioral segments for downstream commercial analytics. Segmentation of this type is frequently used in lifecycle targeting, churn prevention, sales prioritization, and retention strategy.

This is a portfolio-ready version of a group capstone submitted for the BCG RISE 2.0 – Business Data & Analytics program. Sensitive data and group-specific artifacts have been removed. Sample data is used for demonstration.

## Objective

Engineer RFM features from transaction data and assign retailer segments that characterize lifecycle maturity, value contribution, and churn risk.

## Business Value

RFM segmentation enables commercial teams to:

- identify newly onboarded accounts requiring activation
- target high-value accounts for sales coverage
- detect churn-risk cohorts before revenue declines
- quantify revenue concentration by lifecycle stage
- inform portfolio planning and coverage models

The segmentation output also serves as an upstream dataset for churn modeling, CLV estimation, and revenue-at-risk analysis.

## Dataset

The sample dataset consists of anonymized retailer-level transaction records including:

- invoice dates
- SKU-level sales details
- quantities and invoice values
- discounts and margins

Sample data is included for reproducibility:

- data/transactions_sample.csv

No confidential or identifiable fields are present.

## Methodology

The analytical workflow consists of:

1. Data loading and validation
2. Retailer-level aggregation
3. RFM feature engineering
4. RFM scoring
5. Segmentation logic
6. Lifecycle distribution and insights

## Segmentation Logic

Retailers are classified into eight lifecycle cohorts:

| Segment             | Description                                      |
|---------------------|--------------------------------------------------|
| VIP                 | recent, frequent, and high value                 |
| Loyal               | consistent repeat purchasing                     |
| Potential Loyalist  | early repeat activity                            |
| New                 | newly onboarded                                  |
| Need Attention      | moderate engagement                              |
| Risk of Churn       | declining recent activity                        |
| Hibernating         | long inactive                                    |
| Lost                | fully inactive                                   |

## Lifecycle Distribution (Sample Data)

Using sample data (n = 100 retailers):

- 48% early lifecycle (New + Potential Loyalist)
- 24% mature and engaged (Loyal + VIP)
- 21% retention/reactivation opportunities (Risk of Churn + Hibernating + Lost)
- 7% transitional (Need Attention)

This suggests strong onboarding volume with upside to accelerate the maturation of early cohorts into high-value segments.

## Downstream Use Cases (Not Shown in This Portfolio Version)

In the original capstone, segmentation was merged with account-level fields for downstream work, including:

- churn scoring
- CLV estimation
- revenue-at-risk quantification
- portfolio and coverage optimization
- commercial activation planning

This repository focuses on RFM feature engineering and segmentation.

## Repository Structure
```text
bcg_retailer_churn_analysis/
│
├── notebooks/
│   └── rfm_scores.ipynb
│
├── data/
│   └── transactions_sample.csv
│
└── README.md
```

## Technical Stack

Languages and Libraries:

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn

Skills Demonstrated:

- data preprocessing
- feature engineering
- cohort segmentation
- exploratory analysis
- insight generation
- reproducible notebook design

## How to Run

Install dependencies:
pip install -r requirements.txt

Execute notebook:
notebooks/rfm_scores.ipynb

Relative paths are used for portability.

## Role and Contribution

The original capstone was executed as a team project. My contribution focused on:

- data cleaning and preprocessing
- retailer-level aggregation
- RFM scoring logic
- behavioral segmentation
- insight development

All content in this repository reflects work completed personally for portfolio purposes.

## Author

Alex Xu  
Entry-Level Data Analyst (Singapore)
