# Healthcare Operations & Billing Intelligence — Summary Report

## Dataset after cleaning
- Starting rows: 55,500
- Exact duplicates removed: 534
- Negative billing rows removed: 108
- Analysis rows: 54,860
- Missing values in the raw file: 0

## Cleaning choices
- No mean / median / mode fill, because nothing was missing.
- Duplicates dropped to stop double counting.
- Negative bills dropped because they are invalid, not blank.
- Dates converted to datetime so length of stay and month trends work.
- Text stripped so categories do not split by extra spaces.

## New columns
Length_of_Stay, Admission_Year, Admission_Month, Admission_Month_Name, Admission_Quarter, Age_Group, Billing_Band, weekday and weekend flags.

## Headline numbers
- Typical stay: 15 days (mean about 15.5, max 30)
- Typical bill: about $25,540 (mean and median almost equal)
- Top volume condition: Arthritis
- Top total-billing condition: Diabetes
- Largest age group: 66+
- Busiest months: July and August

## What this means
Demand and revenue are diversified. Admission type is not a strong cost splitter in this file. Bed time and inconclusive tests are the clearer operational pressure points.
