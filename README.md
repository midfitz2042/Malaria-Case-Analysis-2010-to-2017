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

# Attributes of the Data
# Visualization
# Analysis
# Recommendation
