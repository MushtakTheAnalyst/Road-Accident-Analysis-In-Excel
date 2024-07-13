# Road_Accident_Analysis
Road accident analysis in the UK for 2021 and 2022 dashboard using microsoft excel


## Project Description
Road safety is a significant concern impacting communities worldwide. In this project, I have developed a Road Accident Analytics Dashboard, a robust tool designed to analyze and visualize road accident data for the years 2021 and 2022. This Excel-based dashboard provides stakeholders with critical insights, enabling them to make data-driven decisions and promote safer roads.


## Goal
The goal of this project is to analyze traffic accident data and identify key trends and insights related to casualties. By doing so, the project aims to inform policy and decision-making related to road safety, and ultimately help reduce the number of casualties caused by accidents.


## Project Requirement
The goal of this Excel project is to develop a Road Accident Dashboard for the years 2021 and 2022, delivering essential insights to clients using a dataset containing 21 fields and 307,000 records. The insights will be represented through two categories of KPIs: Primary KPIs and Secondary KPIs.

#### Primary KPIs:
- Total casualties post-accident
- Total casualties by accident severity and their percentage, and vehicle type maximum casualties.

#### Secondary KPIs:
- Total casualties categorized by vehicle type
- Monthly trend comparing casualties for the current and previous years
- Maximum casualties by road type
- Distribution of total casualties by road surface
- Correlation between casualties based on Area/Location and Day/Night


## Stakeholders List
- Ministry of Transport
- Road Transport Department
- Police Force
- Emergency Service Department
- Road Safety Corps
- Transport Operators
- Traffic Management Agencies
- Public
- Media


## Data Structure
The dataset is in Excel (.xlsx) format with 307,974 rows and 21 columns. It contains accident details with fields like accident_index (unique for every data entry recorded), accident date, location details, accident_severity, number_of_casualties, road_type, vehicle_type, and others.


## Data Source
The dataset can be found [here](https://docs.google.com/spreadsheets/d/1R_uaoZL18nRbqC_MULVne90h3SdRbAyn/edit?usp=sharing&ouid=115582851948476680193&rtpof=true&sd=true)


## Data Cleaning and Transformation

1. The dataset underwent was analyzed in Microsoft Excel to enhance comprehension and identify areas requiring cleaning before analyzing. Notable issues included blank entries and spelling errors. Specifically, the ‘Accident_Severity’ and ‘Junction_Control’ columns included errors such as ‘Fetal’ instead of ‘Fatal’ and ‘Auto traffic sigl’ instead of ‘Auto traffic signal’.

2. The raw data was duplicated into a new sheet, and labeled ‘Data Worksheet.’ The subsequent cleaning procedures were executed on this dedicated sheet, comprising:
 - The Dataset columns were spaced to get a full view
 - Each column was checked for anomalies and any error
 - Blank cells in the columns 'Road_Surface_Conditions' and 'Road_Type' was grouped as "Others" instead of removing the black cells
 - All errors were corrected using the Find and Replace function in Excel
 - Made sure data is consistent and clean with respect to data type, data format and values used
 - Creating 2 new attributes 'Year' and 'Month' were added for logical and easy interpretation of dataset


## Data Processing

Part of the requested KPIs by the client is to showcase the dashboard in monthly and yearly insight, but from our data, we only have an Accident_Date column with the full date for each data entry. Therefore, there is a need to create month and year columns to get the requested insight. The process of doing this is as follows;

1. Create two blank columns, and name them ‘Month’ and ‘Year’ respectively

2. Use the Excel Text function to extract the month and year from the Accident_Date column.
 - =TEXT(B2, “mmm”) for the newly created ‘Month’ column
 - =TEXT(B2, “yyyy”) for the newly created ‘Year’ column


## Data Analysis

#### Primary Key Performance Indicators (KPIs)

- The Excel-Pivot Table was utilized to determine the total number of casualties after the accident in 2021 and 2022.
- The Accident_Severity is of 3 types- Fatal, Serious and Slight. PivotTable was utilized to determine the total number of casualties for each Accident_Severity type, and the Excel function was used to calculate the percentage of total casualties for each Accident_Severity type.
- The same PivotTable was used to determine the Vehicle_Type with maximum casualties.

#### Secondary Key Performance Indicators (KPIs)

- Categorized total casualties based on vehicle types using Excel PivotTable, and casualties for agricultural vehicles, cars, buses, vans, bikes, and others were identified. This breakdown facilitates a detailed understanding of the impact across various vehicle categories.
- Utilized Excel Pivot Table to compare monthly casualties for the current and previous years. This analysis helps identify patterns, seasonality, and potential contributing factors to accidents with time.
- Identified and analyzed the road types associated with the highest casualties. Excel Pivot Table was instrumental in summarizing and visualizing this data.
- Utilized Pivot Table to break down casualties based on road surface conditions. This analysis provides insights into the impact of road conditions on accident severity.
- Excel PivotTable was employed to analyze the correlation between casualties' location and time of day. Understanding the relationship between these variables contributes to targeted safety measures, especially in specific areas.


## Visualization and Dashboard Overview

1. Visualization:

A dedicated ‘Data Analysis’ sheet was created for comprehensive data visualization. Excel’s ‘Insert Function’ feature was utilized to pick suitable charts for each table derived from PivotTable data analysis.

- Primary KPIs: Doughnut charts were employed to visualize and represent primary KPIs. The charts were formatted for clarity, ensuring a clean and easily interpretable presentation.
- Secondary KPIs: Different visualization tools, including Doughnut chart, Treemap, Line graph, and Bar chart, were utilized to convey insights from secondary KPIs.

  
2. Dashboard:

An interactive dashboard with key features to enhance usability and understanding was developed.

- The timeline button was integrated to visualize road accidents in 2021 and 2022 separately or collectively. This enables a more detailed examination of trends and patterns over each year.
- Slicer functionality was incorporated into the dashboard, using Rural/Urban categorization as a filter. This allows users to view the dashboard based on specific KPIs and choose between Urban, Rural, or overall perspectives for a targeted analysis.
- The dashboard is intricately linked with the ‘Data Analysis’ sheet, and providing seamless navigation to internet resources. This integration ensures easy mobility and quick access to related information. This can be interacted with with the use of icons on the left-hand side of the dashboard.


## Key Insights

**Total Casualties Analysis:** The dashboard reveals an alarming 417,883 casualties occurred due to accidents over the two-year period.

**Peak Months:** Casualties were slightly higher in 2021 compared to 2022. The highest number of casualties occurred in October and November in both years, while the lowest casualties were in January and February.

**Casualties by Vehicle Type:** Car accidents accounted for the majority of casualties, contributing to 79.8% of the total. Casualties were minimal in accidents involving other vehicle types.

**Casualties by Accident Severity:** Slight severity accidents accounted for the majority of casualties (84.1%), while fatal severity casualties were only 1.7%.

**Road Type Analysis:** The highest number of casualties occurred on single carriageway roads (309.7K), and the lowest on slip roads (4.7K).

**Casualties Distribution by Road Surface:** The majority of casualties (66.9%) occurred on dry road surfaces.

**Casualties Relation by Area/Location:** Urban areas accounted for 61% of the casualties after accidents.

**Casualties Distribution by Light Condition:** 73% of casualties occurred during daylight conditions.


## Recommendations

1. **Focus on High-Risk Periods:** By comparing casualty trends between the current and previous years on a monthly basis, the dashboard identifies critical periods in October and November. Traffic police and other stakeholders should increase safety measures and monitoring during these high-risk months.

2. **Target Car Drivers:** Since car drivers account for the bulk of casualties, they should be the focus of awareness campaigns, strict monitoring, and periodic check-ups on safe driving.

3. **Improve Single Carriageway Roads:** Extra safety measures should be implemented on single carriageway roads, and wherever possible, these roads should be upgraded to double lanes.

4. **Enhance Road Surface Conditions:** Understanding casualty distribution based on different road surface conditions helps pinpoint areas where road maintenance and surface improvements are essential.

5. **Interventions in Urban Areas:** Urban areas should be targeted for specific interventions to improve road safety, particularly during daylight hours.


## Conclusion

The Road Accident Analytics Dashboard facilitates data-driven decision-making, enabling stakeholders to implement evidence-based decisions that enhance road safety. It serves as a valuable tool for policymakers, traffic authorities, and police departments alike.
