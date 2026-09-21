# HR Attrition Analytics Dashboard (Power BI)

An end-to-end analysis of employee attrition: requirements, data model, DAX measures, dashboard, and recommendations.

## Business problem
237 of 1,470 employees have left (16.1% attrition). Leadership lacks a clear view of where attrition is concentrated and what drives it. This project delivers a Power BI dashboard to guide retention actions.

## Dataset
IBM HR Employee Attrition dataset (Kaggle): 1,470 employees, 35 fields. The data is synthetic and has no date field, so this project demonstrates method, not real-world conclusions. See the [data notes](data/README.md).

## Approach
Followed a 10-stage analytics life cycle: business understanding, data acquisition, profiling and cleaning, modelling, exploration, measures and validation, report design, insights, review, and deployment. See the [life cycle document](docs/HR_Attrition_Analytics_Lifecycle.pdf).

## Data model
Star schema: one fact table at employee grain plus dimensions for department and role, education, employee profile, age and salary bands, and ratings. See the [model notes](model/README.md).

## Key findings
1. **Overtime is the strongest driver.** Overtime staff leave at 30.5% vs 10.4% for others and account for 54% of leavers. If their rate matched the rest, about 84 fewer people would leave and the overall rate would fall to about 10.4% (an illustration, not a forecast).
2. **Risk is concentrated at entry level.** Job Level 1 has a 26.3% rate and accounts for 60% of leavers (143 of 237).
3. **Early tenure and youth matter.** First-year employees leave at about 35%, and under-25s at about 36%.
4. **Rate and volume differ.** Sales Representatives have the highest rate (about 40%); Laboratory Technicians have the most leavers (62).
5. **High performers leave at the same rate as others** (16.4% for rating 4 vs 16.1% for rating 3).

More detail is in the [insights folder](insights/README.md).

## Recommendations
- Review overtime and workload in Level 1 and low-income roles.
- Strengthen first-year onboarding and check-ins.
- Review pay in the bottom income band.
- Target retention actions at Sales Representatives and Laboratory Technicians.

## Limitations
Synthetic, imbalanced data; no date field, so no trends; findings are associations, not causes; some groups are small, so group sizes are shown.

## Project documentation
- [Business Requirements Document](docs/HR_Attrition_Dashboard_BRD.pdf)
- [Data Analytics Life Cycle](docs/HR_Attrition_Analytics_Lifecycle.pdf)
- [User Story Requirements](docs/HR_Attrition_User_Stories.pdf)

Editable Word versions are in the [docs folder](docs/).

## Repository structure
- `docs/`: BRD, life cycle, user stories
- `data/`: data source notes
- `model/`: schema diagram and DAX measures
- `report/`: Power BI file and screenshots
- `insights/`: findings and recommendations

## Tools

![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-1F3864?style=for-the-badge)
![Power Query](https://img.shields.io/badge/Power_Query-2F5496?style=for-the-badge)
![Kaggle](https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)
![Word](https://img.shields.io/badge/Word-2B579A?style=for-the-badge&logo=microsoftword&logoColor=white)
![Markdown](https://img.shields.io/badge/Markdown-000000?style=for-the-badge&logo=markdown&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)

## Next steps
Predictive attrition risk model; synthetic hire date for trend analysis.

## Author
[Ntiyiso Ndhlovu] | [https://www.linkedin.com/in/ntiyiso-ndhlovu-840048129/]
