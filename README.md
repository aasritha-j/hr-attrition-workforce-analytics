# hr-attrition-workforce-analytics
Power BI HR dashboard — Snowflake schema, RLS, What-if parameters, DAX

## Overview
An end-to-end Power BI solution analysing employee attrition and workforce trends using the IBM HR Analytics dataset (1,470 employees, 35 attributes). Built with a production-grade snowflake schema, advanced DAX measures, row-level security, and an interactive what-if scenario planner — demonstrating the full BI stack from data modelling to executive reporting.

## Dashboard Pages

### Page 1 — Attrition Overview
Executive summary of attrition across the organisation with drill-down by department, age band, job role, tenure, and satisfaction score.

<img width="607" height="340" alt="image" src="https://github.com/user-attachments/assets/e7126eef-3fe4-46ae-9284-fe4e2724fea7" />

**Key visuals:**
- 4 KPI cards — Total Employees, Total Attrition, Attrition Rate, Average Tenure
- Attrition by Department, Age Band, Job Role, Tenure Band, Job Satisfaction

**Key insight:** 
Sales Representatives have the highest attrition at 39.8%. Employees in their first year are 3x more likely to leave than those with 5+ years tenure.
<img width="609" height="341" alt="image" src="https://github.com/user-attachments/assets/a565e199-8379-479d-ac4c-c46c599137a4" />


### Page 2 — Workforce Analytics
Deep dive into headcount composition, salary distribution, and satisfaction heatmap by department.

<img width="608" height="340" alt="image" src="https://github.com/user-attachments/assets/3a755012-944f-470f-bf9c-14568ca6789d" />

**Key visuals:**
- 4 KPI cards — Active Employees, Avg Monthly Income, Avg years at company, YTD Exits
- Avg Monthly Income by Job Role (bar chart)
- Job Satisfaction Heatmap — Department × Satisfaction Score (Matrix with gradient conditional formatting)
- Avg Income by Education Level (column chart)

**Key insight:** 
Sales department has the lowest satisfaction scores across all 4 satisfaction dimensions, directly correlating with its highest attrition rate.


### Page 3 — Scenario Planner
Interactive what-if analysis allowing HR leaders to model the impact of salary increases, new hires, and training investments on projected attrition.

<img width="609" height="295" alt="image" src="https://github.com/user-attachments/assets/2185fd49-75cd-4d61-bf5b-98d4d37abd38" />

**Key visuals:**
- 3 interactive what-if sliders — Salary Increase %, New Hires Planned, Training Budget ($K)
- 4 dynamic KPI cards updating in real time — Projected Headcount, Salary Cost Impact, Projected Attrition Rate, Attrition Reduction
- Current vs Projected attrition comparison

**Key insight:** 
A 10% salary increase combined with $200K training investment is projected to reduce attrition by 4.2pp — saving approximately $3.8M in replacement costs annually.


## Data Model — Snowflake Schema

## Tools & Technologies

| Tool | Usage |
|---|---|
| Power BI Desktop | Report development, DAX, data modelling |
| Power Query (M) | Data transformation, dimension table creation |
| DAX | Measures, calculated columns, what-if logic |
| IBM HR Dataset | Source data (Kaggle) |

## Dataset
**IBM HR Analytics Employee Attrition & Performance**
- Source: [Kaggle]([https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset))
- Rows: 1,470 employees
- Columns: 35 attributes
- File: `WA_Fn-UseC_-HR-Employee-Attrition.csv`

## Key Business Insights
1. **Overall attrition rate is 16.1%** — above the industry benchmark of 10–12%
2. **Sales Representatives** have the highest attrition at 39.8% — nearly 2.5x the company average
3. **First-year employees** are the highest risk group — immediate onboarding intervention recommended
4. **Low job satisfaction (Score 1)** correlates with 22.8% attrition vs 9.0% for Score 4
5. **Salary increase of 10% + $200K training** projected to reduce attrition by 4.2pp saving ~$3.8M annually


## How to Run
1. Clone this repository
2. Download the dataset from Kaggle (link above)
3. Open `HR_Attrition_Dashboard.pbix` in Power BI Desktop
4. If prompted, update the data source path to your local CSV file
5. Click **Refresh** to load data


## Author
**[Aasritha Jasty]** — [LinkedIn](www.linkedin.com/in/aasrithajasty01) | [GitHub](https://github.com/aasritha-j)
