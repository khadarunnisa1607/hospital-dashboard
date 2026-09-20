# hospital-dashboard
An end-to-end data analytics project analyzing 1,000 hospital patient records to uncover cost, readmission, and satisfaction trends — built with SQL and Power BI.
<img width="1043" height="582" alt="image" src="https://github.com/user-attachments/assets/af6354f1-1f99-4dbe-b13f-ea0b648efd2f" />

#Project Overview

This project simulates a real hospital operations analytics engagement: validating raw patient data, computing KPIs independently in SQL, and building an interactive executive dashboard in Power BI for hospital leadership.

Dataset: 1,000 patient records (Jan 2023 – Jan 2024) across 6 departments, 7 diagnoses, 4 regions, and 3 insurance types.

#Tools Used

MySQL — data validation, KPI computation, data quality checks
Power BI — interactive dashboard with DAX measures, slicers, and custom theming

#Key Findings

-- Orthopedics has the highest average treatment cost (₹1,04,757), ~17% higher than the lowest-cost department, Neurology (₹89,174).
-- Migraine patients have the highest readmission rate (57.1%) — and it's the only diagnosis sitting in the high-cost and high-readmission quadrant, making it a compounding risk worth prioritizing.
-- Government-insured patients cost ~6.5% more on average than Self-Pay patients (₹1,00,585 vs ₹94,432), while patient satisfaction stays flat (2.95–3.06/5) regardless of cost, region, or outcome.  


#Process

1)Loaded raw patient data into MySQL
2)Validated data quality — checked for duplicates, invalid date sequences, and flagged a synthetic-data indicator (age/department independence)
3)Computed all core KPIs independently in SQL before building the BI layer, so dashboard numbers could be cross-checked against a second calculation
4)Built an interactive Power BI dashboard: 5 KPI cards, 5 visuals (including a cost-vs-readmission scatter plot to flag compounding risk), and 4 slicers for live filtering by Region, Department, Insurance Type, and Outcome








