# Healthcare Operations and Billing Intelligence Dashboard

## Project Overview
This project analyses a healthcare admission dataset to understand patient admissions, billing patterns, hospital performance, length of stay, insurance provider trends, and test result outcomes.

## Business Problem
A healthcare provider needs better visibility into operational pressure points and billing drivers across admission types, medical conditions, age groups, and insurers.

Main question: how can admission and billing data identify cost drivers, operational pressure, and planning opportunities?

## Dataset
- File: `healthcare_dataset.csv`
- About 55,500 synthetic hospital visit records (54,860 after removing exact duplicates and invalid negative bills)
- Columns: Name, Age, Gender, Blood Type, Medical Condition, Date of Admission, Doctor, Hospital, Insurance Provider, Billing Amount, Room Number, Admission Type, Discharge Date, Medication, Test Results

## Tools Used
- Python
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook
- GitHub

## Key Skills Demonstrated
- Data loading and inspection
- Data cleaning with written reasons (mean / median / mode / Unknown / drop)
- Feature engineering
- GroupBy aggregation
- Filtering and sorting
- Visualisation
- Business interpretation

## Key Business Questions
1. Which medical conditions have the highest admission volume?
2. Which conditions generate the highest total billing?
3. Which admission types have the highest average billing?
4. Which patient groups stay longest in hospital?
5. How do test results vary by condition?

## Key Findings
- Admissions are spread across six conditions (Arthritis, Diabetes, Hypertension, Obesity, Cancer, Asthma), not one dominant disease.
- Diabetes has the highest total billing; average bills are close across conditions.
- Elective, Urgent, and Emergency average bills are almost the same.
- Typical length of stay is about 15 days (range 1-30).
- July-August are the busiest months; February is lowest.
- Inconclusive and abnormal tests are common in every condition.
- Five insurers share volume fairly evenly.
- Hospital names are too fragmented for fair hospital ranking.

## Recommendations
- Plan capacity for several chronic conditions together.
- Do not manage cost using admission type alone.
- Review long-stay patients around day 15.
- Track inconclusive tests as a quality KPI.
- Cover all five major payers in contract and denial work.
- Standardise hospital names at data entry.

## How to run
```bash
pip install pandas matplotlib seaborn jupyter
jupyter notebook healthcare_analysis.ipynb
```

Keep `healthcare_dataset.csv` in the same folder as the notebook.

## Author
Akpos
Inferaq Academy Data Analytics Programme
