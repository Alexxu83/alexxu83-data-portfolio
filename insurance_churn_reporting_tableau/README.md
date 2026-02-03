# Insurance Customer Status & Segmentation Reporting (Tableau)

## Overview
This project presents a reporting and segmentation dashboard built using Tableau to monitor customer service status and key demographic and behavioural segments within an insurance context. The focus is on **data preparation, structured reporting, and insight communication**, rather than predictive modelling.

This repository contains a **portfolio-adapted version** of a data analytics capstone completed as part of the Vertical Institute Data Analytics programme. The content has been streamlined for professional presentation and portfolio use.

---

## Objective
The objectives of this project are to:

- Provide a clear reporting view of customer service status (active vs terminated)
- Segment customers across key attributes such as age, income, tenure, and account value
- Support monitoring and high-level decision-making through visual analysis

The dashboards are designed to reflect how reporting and segmentation can be used in operational reviews and retention-related discussions.

---

## Approach
Key steps in the project include:

- Joining multiple source tables within Tableau  
  (customer, demographic, address, and service status data)
- Performing basic data validation checks for:
  - null values  
  - duplicate records  
  - inconsistent entries
- Creating calculated fields to:
  - standardise customer attributes  
  - derive service status indicators
- Grouping customers into segments based on:
  - age bands  
  - income bands  
  - tenure groups  
  - account value ranges
- Visualising distributions and comparisons using Tableau dashboards

---

## Tools Used
- **Tableau**  
  - data preparation  
  - calculated fields  
  - dashboard development
- **Excel / CSV datasets**  
  - source data format

---

## Outputs
The project produces interactive Tableau dashboards that illustrate:

- Distribution of active vs terminated customers
- Customer segments by demographic and financial attributes
- High-level patterns relevant to customer status monitoring

The Tableau Public dashboard link is included within the project report PDF.

---

## Notes
- The underlying dataset is publicly available and used for demonstration purposes only.
- Raw datasets are **not included** in this repository.
- This project is intended to demonstrate:
  - reporting structure  
  - segmentation logic  
  - communication of insights  
  rather than advanced statistical or machine-learning techniques.

---

## File Structure
```text
insurance_churn_reporting_tableau/
├── README.md
└── Insurance_Churn_Reporting_Tableau_Capstone.pdf
```

---

## How to Use
1.	Review the PDF report for project context, methodology, and visual outputs.
2.	Access the Tableau Public dashboard via the link provided in the report (optional).

---

## Portfolio Context
This project complements a Python-based segmentation workflow (RFM analysis) in the same portfolio by demonstrating BI-focused reporting and dashboarding capabilities alongside reproducible data analysis work.
