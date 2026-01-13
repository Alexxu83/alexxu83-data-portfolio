# Retailer Segmentation Using RFM Analysis

Objective: Perform RFM segmentation on retailer transaction data to identify behavioral cohorts and support downstream commercial analytics.

Business Value: Enables churn risk monitoring, revenue-at-risk estimation, and commercial account prioritization.

---

## Overview

This project uses anonymized retailer transaction data to engineer RFM (Recency, Frequency, Monetary) features and derive behavioral segments. RFM segmentation is commonly used in commercial analytics workflows including:

- churn prediction
- customer lifetime value (CLV)
- retention modeling
- revenue forecasting
- sales prioritization

This is a cleaned portfolio version of a larger group capstone project completed as part of the BCG RISE 2.0 Business Data & Analytics program. Sensitive data and environment-specific artifacts have been removed.

---

## Methodology

The analytical workflow includes:

1. Data loading and cleaning
2. Retailer-level aggregation
3. RFM feature engineering
4. Recency, Frequency, and Monetary scoring
5. Segment assignment
6. Lifecycle interpretation
7. Insights and business recommendations

---

## Repository Structure

rfm-segmentation/
│
├── notebooks/
│   └── rfm_scores.ipynb
│
├── data/
│   └── transactions_sample.csv
│
└── README.md

---

## Technical Stack

Languages and libraries:

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn

Analytical capabilities demonstrated:

- data cleaning and preprocessing
- feature engineering
- cohort segmentation
- exploratory analysis
- insight generation
- reproducible notebook development

---

## RFM Segmentation Logic

Segmentation is based on:

- Recency: days since last transaction
- Frequency: number of transactions
- Monetary: total sales contribution

Final segments include:

| Segment             | Description                                      |
|---------------------|--------------------------------------------------|
| VIP                 | recent, frequent, high-spend customers           |
| Loyal               | consistent repeat customers                      |
| Potential Loyalist  | early repeat purchasing behavior                 |
| New                 | recently onboarded customers                     |
| Need Attention      | moderate engagement, at risk of declining        |
| Risk of Churn       | declining recent activity                        |
| Hibernating         | long inactive                                    |
| Lost                | fully inactive                                   |

---

## Key Observations (Sample Dataset)

Using anonymized data for demonstration:

- 48% of retailers fall within early lifecycle segments (New + Potential Loyalist)
- 24% are mature and engaged (Loyal + VIP)
- 21% represent retention or reactivation opportunities (Risk of Churn + Hibernating + Lost)
- Early lifecycle growth and onboarding acceleration represent the largest opportunity area

---

## Business Implications

The segmentation output provides a foundation for:

- churn risk detection
- revenue-at-risk quantification
- account prioritization for commercial teams
- lifecycle management playbooks
- targeted retention and upsell initiatives

---

## Scope Note

In the original capstone project, this enriched dataset was merged with additional account information for downstream modeling (including churn scoring and revenue prioritization). For portfolio purposes, the scope is intentionally limited to feature engineering and segmentation.

---

## Running the Notebook

To reproduce results:

1. Clone the repository
2. Install dependencies (optional: requirements file)
3. Open and execute `notebooks/rfm_scores.ipynb`

---

## Author

Alex Xu  
Entry-Level Data Analyst (Singapore)  
LinkedIn: https://www.linkedin.com/in/alexxu83
