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
 - The cleaning process is tailored to the requested KPIs by the client
 - Each column was checked for anomalies and any error
 - Blank cells in the columns 'Road_Surface_Conditions' and 'Road_Type' was grouped as "Others" instead of removing
 - All errors were corrected using the Find and Replace function in Excel.

## Data Processing

Part of the requested KPIs by the client is to showcase the dashboard in monthly and yearly insight, but from our data, we only have an Accident_Date column with the full date for each data entry.

Therefore, there is a need to create month and year columns to get the requested insight. The process of doing this is as follows;

Create two blank columns, and name them ‘Month’ and ‘Year’ respectively

Use the Excel Text function to extract the month and year from the Accident_Date column.
=TEXT(B2, “mmm”) for the newly created ‘Month’ column
=TEXT(B2, “yyyy”) for the newly created ‘Year’ column

