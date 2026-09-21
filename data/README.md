# Data

## Source
IBM HR Employee Attrition dataset from Kaggle.
- Link: kagglehub.dataset_download("pavansubhasht/ibm-hr-analytics-attrition-dataset")
- Downloaded: [21 September 2026]
- Size: 1,470 employees, 35 columns
- Quality checks: no missing values, and EmployeeNumber is unique
- The dataset is synthetic (fictional employees), so findings demonstrate method, not real-world conclusions.

## Licence note
The raw CSV is not stored in this repository. Download it from the link above.

## Cleaning steps
1. Removed the constant columns EmployeeCount, StandardHours, and Over18.
2. Created IsAttrition (1 if Attrition is Yes, otherwise 0).
3. Replaced the numeric rating scales (satisfaction, involvement, work-life balance, performance, education) with descriptive labels.
4. Split the data into a fact table and dimension tables (see the model folder).

## Known limitations
- No date field, so time trends cannot be analysed.
- 237 of 1,470 employees have left (16.1%), so the classes are imbalanced.
