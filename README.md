# Malaria-Report-2010-to-2017
This is a Report that sought to analyze Malaria cases and deaths from 107 countries around the world
# Introduction
Malaria is an acute febrile illness caused by Plasmodium parasites, which are spread to people through the bites of infected female Anopheles mosquitoes. It is preventable and curable, however till date, the cases of malaria countinues to rise in soome regions of the world. <br/>
In this project, I carried out an analysis on malaria cases, from 107 countries reporting malaria cases to the World Health Organization from 2010 to 2017.
# Problem Statement
From the dataset gotten, I would like to look at the trend in mlaria cases from 2010 to 2017, the deaths that resulted from these cases over the years, incidence of malaria around the world, the areas that were burdened by these cases. <br/>
This analysis would help both local and international health organizations, stakeholders in the health sector acccess the interventions in the control of malaria over the years ; It would also help guide where more resources to control malaria should be put.
# Data Sourcing
The Dataset for this analysis was gotten from Kaggle <br/>
The dataset consisted of 3 tables consisting of reported numbers, incidence, and estimated number of cases and death from 2010 to 2017 respwctively.
# Data Cleaning in Microsoft Excel and Power Query
## Power Query
The 3 tables from the dataset were first loaded into Power Query

The table that contained reported numbers was then merged with the table that contained incidence per 1000 population at risk. The incidence table was expanded and the desired column was selected.

The resulting table from the above was then merged with the table that contained reported numbers. The reported numbers table was then expanded and the columns containing reported cases and reported deaths were selected.

The merged dataset was then loaded into Microsoft Excel.
## Microsoft Excel
In MS Excel, the dataset was checked for misspellings and the misspellings found were replaced.

Null values in the numeric fields were replaced with "0".

Two columns (Number of Cases, Number of Deaths) that showed the minimum, median and maximum estimated cases in each cell were deleted since they were not going to be used during the visualization process. This was done to optimize performace during visualization.

Column names were replaced with more relateable names

The dataset was checked for duplicate values

The dataset was then copied into another another excel workbook. This was done to reduce the size of the dataset that would be imported into Power BI since 3 tables were merged. Only the merged dataset was copied.

At the end of cleaning, there were 12 columns and 856 rows. The dataset was then imported into Power BI for visualization.

# Attributes of the Data
The following are what each field means:
- Country: The country reporting the cases,death, and incidence
- Year: The Year the cases,death, and incidence were reported
- Estimated_cases_median: Median estimate of the number of cases
- Estimated_cases_min: Minimum estimate of the number of cases
- Estimated_cases_max: Maximum estimate of the number of cases
- Estimated_deaths_median: Median estimate of the number of deaths
- Estimated_deaths_min: Minimum estimate of the number of deaths
- Estimated_deaths_max: Maximum estimate of the number of deaths
- W.H.O Region: The World Health Organization Region the Country is located
- No. of cases_incidence: The number of cases per 1000 population at risk
- Reported_No_of_cases: The number of cases reported to the World Health Organization
- Reported_No_of_deaths: The number of cases reported to the World Health Organization
# Visualization
All Visualizations for this project were done using Microsoft Power BI

View dashboard here <br/>
Interact with report here
# Analysis
# Recommendation
