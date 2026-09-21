
# Data model

The report is built on a star schema: one fact table at employee grain, surrounded by dimension tables.

## Tables
- FactEmployee: one row per employee (1,470 rows), with IsAttrition and the numeric measures such as income, tenure, and years since promotion
- DimDepartmentRole: 11 department and job role combinations (some roles span departments, so the key is the combination)
- DimEducationField: education field and education level labels
- DimEmployeeProfile: gender, marital status, business travel, overtime, and stock option level
- DimAgeGroup and DimSalarySlab: editable band definitions
- DimRating: labels for the 1-4 rating scales

## Files
- star-schema.png: model diagram
- measures.md: DAX measure definitions

## Validation
Totals reconcile to the source data: headcount 1,470, leavers 237, attrition rate 16.1%.
