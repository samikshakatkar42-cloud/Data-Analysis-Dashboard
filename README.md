# Loan-Default  – (Interactive Dashboard creation using Power BI)
## Description 
This project demonstrates a complete end-to-end Business Intelligence solution using Power BI, SQL Server, and Power BI Dataflows to analyse loan default Behaviour.
The goal is to help stakeholders understand loan distribution, default rates, risk patterns, and customer demographics to support data-driven lending decisions.
The project covers the entire BI lifecycle — from data ingestion and transformation to advanced DAX calculations, data validation, visualization, and automated refresh.

## DataSet used 
- <a href=https://github.com/samikshakatkar42-cloud/Data-Analysis-Dashboard/commit/db06e072e89978686478e146f5e54c58b9ef4cad

## Project Implementation Steps
 Environment Setup
•	Downloaded, installed, and configured Power BI Standard Mode Gateway
•	Installed and configured Microsoft SQL Server
•	Imported raw loan data into SQL Server tables

## Data Integration & Dataflow
•	Created Power BI Dataflow using Power BI Service
•	Connected SQL Server as the data source
•	Implemented centralized data transformation logic
•	Enabled reusability and consistency across reports

## Data Modeling & Power Query
•	Imported data into Power BI Desktop from Dataflow
•	Defined column descriptions and dataset documentation
•	Verified data types and data profiling
•	Cleaned and transformed data using Power Query Editor

## Report Design & Page Layout
•	Renamed report pages for clarity
•	Inserted shapes and visual headers for professional layout
•	Designed user-friendly dashboards with consistent formatting

## Key Analysis & DAX Measures
🔹 Loan Amount Analysis
•	Loan Amount by Purpose
o	DAX Used: SUMX, FILTER, NOT, ISBLANK
•	Average Loan Amount by Employment Type
o	DAX Used: CALCULATE, AVERAGE, ALLEXCEPT

🔹 Default Rate Analysis
•	Default Rate by Employment Type
o	DAX Used: CALCULATE, COUNTROWS, ALLEXCEPT, FILTER, DIVIDE
•	Default Rate by Year
o	Includes data validation checks
•	Year-Over-Year (YoY) Default Loan Change
o	Custom DAX Measure for trend analysis

🔹 Age & Demographic Insights
•	Average Loan Amount by Age Group
o	DAX Used: AVERAGEX, VALUES
•	Average Loan Validation by Age Group
•	Donut Chart: Average Loan Amount by Age Group & Marital Status
•	Credit Score Category vs Loan Amount
•	Loan Amount for Middle-Aged Adults
o	By Mortgage & Dependent Status
o	Includes clustered column chart with validation

🔹 Advanced Metrics
•	Median Loan Amount
o	DAX Used: MEDIANX
•	Median Loan Amount by Credit Score Category
•	YTD Loan Amount
o	By Credit Score Bins & Marital Status
•	YoY Loan Amount Change
o	Line charts for trend visualization

🔹 Advanced Visual Analytics
•	Decomposition Tree
o	DAX Used: SWITCH
o	Enables drill-down analysis of default drivers

## Data Validation
•	Cross-validated:
o	Default rates
o	Median & average loan calculations
o	Visual totals vs DAX results
•	Ensured accuracy and reliability of insights

## Automation & Refresh
•	Configured Scheduled Refresh for Dataflow
•	Enabled Incremental Refresh
o	Improves performance
o	Handles large datasets efficiently
