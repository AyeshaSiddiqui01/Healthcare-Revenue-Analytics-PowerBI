# Interactive Healthcare Operations Dashboard (Power BI)

An end-to-end analytics project built using Power BI and patient-level data from Johns Hopkins University.
This dashboard provides a 360° view of clinical performance, operational efficiency, and financial insights within a healthcare setting.
It integrates data from diagnoses, procedures, lab results, encounters, and billing records to help hospitals make informed, data-driven decisions.

# About the Dataset

The dataset combines multiple healthcare data sources, including Patient demographics, Diagnoses & chronic conditions, Lab test results, Procedure details, Encounter and visit information, Billing and revenue data

A custom Risk Stratification Model groups patients into Low, Medium, and High Risk categories using factors such as Age, Chronic diseases, and Abnormal lab biomarkers
Although fewer in number, high-risk patients contribute significantly to total billing and have longer hospital stays, highlighting opportunities for proactive care management.

# Data Model & Relationships
Following Tables are used

epic_patients – patient demographics, age

encounters – patient encounters and visit data

epic_billing – billing charges, CPT/procedure codes, posting dates

diagnosis – diagnosis codes and descriptions

lab_results – abnormal lab indicators

Calculated measures (Power BI DAX)

# Key Relationships

epic_patients[PAT_ID] → encounters[PAT_ID]

encounters[PAT_ENC_CSN_ID] → epic_billing[PAT_ENC_CSN_ID]

encounters[PAT_ENC_CSN_ID] → diagnosis[PAT_ENC_CSN_ID]

This enables multi-table analytics such as risk scoring and revenue aggregation.

# What This Dashboard Helps Solve

This dashboard supports healthcare teams in:

Identifying high-risk, high-cost patient groups

Optimizing bed utilization and throughput

Enhancing care quality with data-driven insights

Monitoring clinical and financial performance

Supporting value-based care and preventive care strategies

# Key Insights from the Analysis

High-risk patients generate significantly higher revenue due to complex health needs.

Chronic conditions like diabetes and heart failure drive major treatment costs.

Departments with longer LOS can target workflow improvements.

Monthly revenue patterns highlight seasonal trends and utilization cycles.

# Files Included in This Repository

Project.pbix file

# Dashboard Preview

<img width="663" height="342" alt="Screenshot 1" src="https://github.com/user-attachments/assets/85c51a59-b20f-4600-8d4b-d2ad7b3ff99e" />

<img width="635" height="338" alt="Screenshot 2" src="https://github.com/user-attachments/assets/85b17a98-04a8-45c3-9da2-b1a0aa0c97c5" />

<img width="632" height="335" alt="Screenshot 3" src="https://github.com/user-attachments/assets/94aef175-5b8b-4e3c-a4aa-7d7218531e67" />



# Author
Ayesha Siddiqui |
Data Analyst
