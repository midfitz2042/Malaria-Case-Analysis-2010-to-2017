# Malaria-Report-2010-to-2017
This is a Report that sought to analyze Malaria cases and deaths from 107 countries around the world
# Introduction
Malaria is an acute febrile illness caused by Plasmodium parasites, which are spread to people through the bites of infected female Anopheles mosquitoes. It is preventable and curable, however till date, the cases of malaria countinues to rise in soome regions of the world. <br/>
In this project, I carried out an analysis on malaria cases, from 107 countries reporting malaria cases to the World Health Organization from 2010 to 2017.
# Problem Statement
From the dataset gotten, I would like to look at the trend in malaria cases from 2010 to 2017, the deaths that resulted from these cases over the years, incidence of malaria around the world, the areas that were burdened by these cases. <br/>
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

Upon importing the dataset into Power BI, the following measures were created using Data Analysis Expressions(DAX); This was done to optimize performance of the visuals:
- Average Incidence
- Estimated Mortality Rate
- Maximum Estimated Cases
- Median Estimated Cases
- Minimum Estimated Cases
- Maximum Estimated Deaths
- Median Estimated Deaths
- Minimum Estimated Deaths
- Total Reported Cases
- Total Reported Deaths
# Analysis
## Key Indices
From 2010 to 2017, there was an average incidence of 92 cases of malaria per 1000 population at risk. There were 552 million reported cases of malaria and about 913 thousand deaths with a mortality rate of 0.23%(23 deaths in every 10,000 cases of malaria). The maximum, median and minimum estimated cases were 2.7 billion, 1.8 billion, and 1.2 billion respectively. The maximum, median, and minimum estimated deaths were 5.3 million, 4.0 million, and 2.3 million respectively.

![image](https://user-images.githubusercontent.com/107150730/184416722-1c538fa2-a94e-4e46-a8a7-184cd68fd8b0.png)

## Yearly Trends in Cases and Deaths from malaria
From 2010 to 2017, there was a gradual increase in malaria cases. The year 2017 accounted for the most cases with 120 million reported cases of malaria as compared to 2010 with 26 million cases. Although, the reported cases did increase over the years, part of this could still be attributed to increased surveillance and case diagnosis over the years.

Although the cases of malaria increased, there was a staggering 63% decrease in malaria deaths from 2010 to 2017. There were 96,561 deaths in 2017 compared to 2010 where there were 155,002 reported deaths. The decrease in deaths can be attributed to increased quality of case management (diagnosis and treatment), increased use of insecticide treated mosquito nets, increased intermittent preventive treatment in pregnancy (which reduced placental infection, clinical malaria, maternal anaemia, fetal anaemia, low birth weight and neonatal mortality from malaria during pregnancy), and intermittent residual spraying.

The average incidence per 1000 population at risk has also shown a decrease from 2010 (101 cases). There has been no more than 90 cases per 1000 population at risk from 2014 to 2017.
# Recommendation
