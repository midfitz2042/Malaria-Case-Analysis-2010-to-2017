# Malaria-Case-Ananlysis-2010-to-2017

![Home page malaria_1](https://user-images.githubusercontent.com/107150730/184448588-29e7b414-7d97-4299-a4e3-7084a40440b7.jpg)

# Introduction
**Malaria** is an acute febrile illness caused by **Plasmodium** parasites, which are spread to people through the bites of infected female **Anopheles** mosquitoes. It is preventable and curable, however till date, the cases of malaria countinues to rise in some regions of the world. Some population groups are at considerably **higher** **risk** of contracting malaria and developing severe disease: infants, children under 5 years of age, pregnant women and patients with HIV/AIDS, as well as people with low immunity moving to areas with intense malaria transmission such as migrant workers, mobile populations and travellers. <br/>
In this project, I carried out an analysis on malaria cases, from **107** countries reporting malaria cases to the **World Health Organization** from **2010** to **2017**.
# Problem Statement
From the dataset gotten, I would like to look at the **trend** in malaria cases from 2010 to 2017 in 107 countries that reported cases of malaria, the **deaths** that resulted from these cases over the years, **incidence** of malaria around the world, the **areas** that were burdened by these cases. <br/>
This analysis would help both local and international health organizations, stakeholders in the health sector assess the interventions in the control of malaria over the years ; It would also help guide where more resources to control malaria should be put.
# Data Sourcing
The Dataset for this analysis was gotten from [**Kaggle**](https://www.kaggle.com/datasets/imdevskp/malaria-dataset?select=incidence_per_1000_pop_at_risk.csv) <br/>
The dataset consisted of **3 tables** containing reported numbers; estimated number of cases and death from 2010 to 2017; Incidence per 1000 population at risk from 2010 to 2018
# Data Cleaning in Microsoft Excel and Power Query
## Power Query
The 3 tables from the dataset were first loaded into Power Query

![loading power query](https://user-images.githubusercontent.com/107150730/184446908-64e4eff0-5093-4989-8c51-a6ddd01fda13.jpg)

The table that contained **estimated numbers** was then merged with the table that contained **incidence** per 1000 population at risk. The incidence table was **expanded** and the desired column was selected.

![first merge](https://user-images.githubusercontent.com/107150730/184447034-a6a05215-d243-4318-86b3-4a341f5cecaf.jpg) ![selecting incidence column to expand](https://user-images.githubusercontent.com/107150730/184447085-eab27fc8-8331-4904-8be3-ab7e553ec4ac.jpg)

The resulting table from the above was then merged with the table that contained **reported numbers**. The reported numbers table was then expanded and the columns containing **reported cases** and **reported deaths** were selected.

![second merge query](https://user-images.githubusercontent.com/107150730/184447559-22f32425-6365-46df-9aad-8e479d08e42f.jpg) ![image](https://user-images.githubusercontent.com/107150730/184447884-36b66cdb-7cc3-4745-a3e5-7de6709f848f.png)

The merged dataset was then loaded into Microsoft Excel.
## Microsoft Excel
In MS Excel, the dataset was checked for **misspellings** and the misspellings found were replaced.

![Correcting country name](https://user-images.githubusercontent.com/107150730/184446430-c150128a-cfe1-4f88-ad9f-335aa7eecf10.jpg)

Null values in the numeric fields were replaced with "**0**".

![Replacing blank with zero](https://user-images.githubusercontent.com/107150730/184446465-a4c595d8-5ab0-4ea2-87c5-4a082ff922d2.jpg)

Two columns (Number of Cases, Number of Deaths) that showed the minimum, median and maximum estimated cases in each cell were **deleted** since they were not going to be used during the visualization process. This was done to **optimize** performace during visualization.

![deleted columns](https://user-images.githubusercontent.com/107150730/184446551-61392513-0bb6-40ec-90bf-f263e3c67ebe.jpg)

Column names were replaced with more relateable names.

The dataset was checked for duplicate values.

![checking for duplicates](https://user-images.githubusercontent.com/107150730/184446593-2e7d2e4e-05a9-4c4c-bce0-2e485c2cabeb.jpg)

The dataset was then copied into another another excel workbook. This was done to reduce the size of the dataset that would be imported into Power BI since 3 tables were merged. Only the merged table was copied.

At the end of cleaning, there were 12 columns and 856 rows. The dataset was then imported into Power BI for visualization.

![No  of columns after cleanng](https://user-images.githubusercontent.com/107150730/184446711-3b2b2a12-fbf9-42fc-9503-cf185db61e49.jpg)

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
- W.H.O Region: The World Health Organization Region(W.H.O) the Country is located
- No. of cases_incidence: The number of cases per 1000 population at risk
- Reported_No_of_cases: The number of cases reported to the World Health Organization(W.H.O)
- Reported_No_of_deaths: The number of cases reported to the World Health Organization(W.H.O)
# Visualization
All Visualizations for this project were done using **Microsoft Power BI**

[View dashboard here](https://github.com/midfitz2042/Malaria-Report-2010-to-2017/blob/main/Dashboard_malaria_cases_2010_2017.pdf) <br/>
[Interact with the report here](https://app.powerbi.com/links/M-z-XHJcwI?ctid=a7c50249-c148-4b70-9b9c-6c4b157ec4f5&pbi_source=linkShare)

![Dashboard_malaria_cases_2010_2017_jpeg](https://user-images.githubusercontent.com/107150730/184480143-0c143e05-1b78-4bae-b473-3f156d2d3940.jpg)

Upon importing the dataset into Power BI, the following measures were created using **Data Analysis Expressions**(DAX); This was done to optimize performance of the visuals:
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
From the year 2010 to 2017, there was an average **incidence** of **92** cases of malaria per 1000 population at risk. There were **552 million** reported cases of malaria and about **913 thousand** deaths with a mortality rate of **0.23%**(23 deaths in every 10,000 cases of malaria). The maximum, median and minimum **estimated cases** were 2.7 billion, 1.8 billion, and 1.2 billion respectively. The maximum, median, and minimum **estimated deaths** were 5.3 million, 4.0 million, and 2.3 million respectively.

![image](https://user-images.githubusercontent.com/107150730/184416722-1c538fa2-a94e-4e46-a8a7-184cd68fd8b0.png)

## Yearly Trends in Cases and Deaths from malaria
From **2010** to **2017**, there was a gradual **increase** in malaria cases. The year **2017** accounted for the most cases with **120 million** reported cases of malaria as compared to **2010** with **26 million** cases. Although, the reported cases did increase over the years, part of this could still be attributed to increased surveillance and case diagnosis over the years. Climate change (related fluctuations in rainfall, temperature and humidity) might have contributed to malaria transmission in areas that were not be adequately resourced or prepared to prevent, detect, and treat the disease.

![image](https://user-images.githubusercontent.com/107150730/184446187-810cdaf7-4c84-4d5c-8336-7900bd7afe9b.png)

Although the cases of malaria increased, there was a staggering **63% decrease** in malaria **deaths** from the year 2010 to 2017. There were **96,561** reported deaths in 2017 compared to 2010 where there were **155,002** reported deaths. The decrease in deaths can be attributed to increased quality of case management (diagnosis and treatment), increased use of insecticide treated mosquito nets, increased intermittent preventive treatment in pregnancy (which reduced placental infection, clinical malaria, maternal anaemia, fetal anaemia, low birth weight and neonatal mortality from malaria during pregnancy), and intermittent residual spraying.

![image](https://user-images.githubusercontent.com/107150730/184446051-4d81648d-d760-4845-932b-28926a4b2456.png)

The average **incidence** per 1000 population at risk has also shown a **decrease** from 2010 (**101** cases). There has been no more than **90** cases per 1000 population at risk from the year 2014 to 2017.

![image](https://user-images.githubusercontent.com/107150730/184445917-ad3ef887-261b-40ee-b717-8ff08d098ab5.png)

## Malaria cases by Location
The **Democratic Republic of the Congo** had the highest **reported** cases with **71 million** cases from 2010 to 2017 with **21** deaths per 10,000 cases of malaria. This is followed by **Burkina Faso** with **41 million** reported cases.  The Democratic Republic of the Congo, Burkina Faso, Mozambique, Uganda, and Nigeria accounted for about **50%** of cases in **Sub-Saharan Africa**. **16** countries, all in **Sub-Saharan Africa** accounted for **80%** of all reported cases of malaria.

![image](https://user-images.githubusercontent.com/107150730/184445652-1a05078e-e3ed-43aa-996f-cf96f87f6bca.png)

There was a gradual increase in reported cases among the top 5 countries over the years. From 2014 to 2017, the trend line of **reported** cases for Burkina Faso, Mozambique, and Uganda fell between the trend lines for the **minimum** and **maximum** estimated cases. This could be attributed to increased surveillance and diagnosis of cases. 

![image](https://user-images.githubusercontent.com/107150730/184436088-9e6dd618-6c4c-4d90-9ea2-da51bcc33b2e.png)

![image](https://user-images.githubusercontent.com/107150730/184474125-26bd2cfe-766e-4069-872c-481fae5bd920.png)

**Nigeria** had the highest maximum **estimated** cases with an average of  **80 million** cases per year. Nigeria also had the lowest **reported** cases with an average of **5%** of maximum estimated cases reported per year and zero reported cases in 2011, 2012,  and 2013.

![image](https://user-images.githubusercontent.com/107150730/184436241-297798d3-ec56-431b-bc96-4599851284dc.png)

Among the top 5 countries with the highest estimated cases, the **Democratic Republic of the Congo** had the highest **estimated mortality rate**(**0.21%**) with **21** deaths in every **10,000** cases. This is followed closely by **Nigeria** with a mortality rate of **0.20%**, then **Uganda** and **Mozambique** with a mortality rate of **0.18%**. The top 5 countries with the exception of **India** were from Sub-Saharan Africa. India had the lowest mortality rate(**0.16%**).

![image](https://user-images.githubusercontent.com/107150730/184473964-08a7ea0d-9152-4a32-8b46-a866d370d7d1.png)

**Nigeria** had the highest **estimated death** from the year 2010 to 2017 with **903,368** deaths. This was followed by the **Democratic Republic of the Congo** with **396,790** deaths which was less than **50%** of the deaths in Nigeria. **17** countries with the exception of India accounted for about 80% of estimated malaria deaths. All these countries were from Sub-Saharan Africa.

![image](https://user-images.githubusercontent.com/107150730/184444930-22f45b8d-6d65-42db-a040-f0ba9f000fa6.png)

Most of the malaria cases were in the **W.H.O African region** accounting for **89%** of **estimated cases** of malaria(**1.58 billion** cases), followed by **W.H.O South-East Asia** region with **133 million** cases(**7.45%**) and **Eastern Mediterranean** with **34 million** cases(**1.93%**). The **Western Pacific** had **15 million** cases while the **Americas** had about **13 million** cases. **Europe** had the least estimated cases(**262**).

![image](https://user-images.githubusercontent.com/107150730/184445024-57d62f04-e069-463b-a251-3d69c8645f84.png)

Of the six W.H.O Regions, only **Europe** and **South-East Asia** showed a **decrease** in reported cases over the years. The remaining W.H.O Regions showed a massive increase in cases from the year 2010 to 2017.

The **W.H.O African region** also accounted for **91.83%** of **estimated deaths** from malaria over the years. This was followed by **South-east Asia** with **5.39%**.

![image](https://user-images.githubusercontent.com/107150730/184473820-63a73507-4464-4b5a-83d5-0c889c66c9ab.png)

The **W.H.O African region** is the most affected due to the following reasons: <br/>
- A very efficient mosquito (Anopheles gambiae  complex) is responsible for high transmission.
- The predominant parasite species is Plasmodium falciparum , which is the species that is most likely to cause severe malaria and death.
- Local weather conditions often allow transmission to occur year round.
- The rise of drug resistant malaria in the region.
- Scarce resources and socio-economic instability have hindered efficient malaria control activities.
# Recommendation
Based on the findings of this analysis:
- The Ministry of Health of burdened areas should ensure strict adherence to measures put in place by the World Health Organization for prevention, control, and eradication of malaria.
- There should be a global concerted effort to improve funding for acquisition of malaria drugs, malaria research, and development of new drugs.
- The Food and Drug agencies of various countries and health workers involved in the treatment of malaria cases should ensure standardization of dosage and case diagnosis to reduce cases of drug resisitant malaria.
- The Ministry of Health should ensure there is increased surveillance and sensitization of the public about malaria.
- There should be effort by the government of various countries to stabilize socio-economic activities and increase budget for the health sector.

[Interact with the report here](https://app.powerbi.com/links/M-z-XHJcwI?ctid=a7c50249-c148-4b70-9b9c-6c4b157ec4f5&pbi_source=linkShare)
