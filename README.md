# USA Domestic Stock Market Analysis 
## PURPOSE:
This is a basic stock market analysis tool created as a capstone project for Dev10. The purpose of this project is to analyze the domestic stock market and its top 5 sectors as determined by market capitalization. Vanguard's top 5 ETF index funds were chosen to represent the top 5 sectors in the US. Vanguard's VTI was chosen as the index fund used to represent the US economy. We compare the historical stock prices of VTI to the total US revenue by year for the years 2006-2020 to validate the latter assumption. Several machine learning models were implemented to see if Vanguard's top 5 ETF index funds were valid indicators of economic trends in the US. This was done by using other US economic features as training and testing data. 

## REQUIREMENTS:
This project utilizes Azure Databricks, Microsoft Azure Data Factories and Pipelines, Kafka Producers and Consumers, SQL databases, and Power BI.

## MAINTENANCE:
This was created for an assignment and will likely not be updated after 2/18/2022.

## REPOSITORY FILES:
README.md        

DashboardNapkinsAndFeedback.png: rough sketch of the Power BI dashboard outline

VisualizationsNapkinsAndFeedback.png: rough sketch of specific visualizations for the Power BI dashboard

ERD.jpg: Entity Relationship diagram for how we set-up our SQL database schema

RepeatableETLReport: An ETL document on how to extract, transform, and load data from the Alpha Vantage API into a SQL database

### Code (folder, contents listed below):
  API-Producer.ipynb: Python code used in Azure Databricks for the Producer of our Azure Data Factory.

  Base-Consumer.ipynb: Python code used in Azure Databricks for the Consumer of our Azure Data Factory.

  Capstone Project Report - Super Finance Bros.pbix: PowerBi dashboard/report for a U.S. Stock Market Analysis

  LSTM_Model.ipynb: Python Code on how the LSTM model was created and descriptions about the decisions made for key parameters.

  Linear Regression Assumptions.ipynb: Describes the decisions made about the methodology chosen for the Linear Regression and LassoCV models.

  Linear Regression and LassoCV Model for Capstone Project.ipynb: Python code used to create the Linear Regression and LassoCV models. 

  Visualizations.ipynb: Contains all Python code used for creating the visualizations in Power BI that used Python scripting (with the exception of the Machine Learning Model comparisons and Historical Price vs. Total US revenue visualizations)

  arima.ipynb: Python code for creating the ARIMA model and descriptions about the decisions made for key parameters.

  model comparisons.ipynb: Python code used in constructing the Machine Learning Model Comparison visualization in Power BI.

### Project Specifications (folder, contents listed below)

  Executive Summary.pdf: details the overall scope of this project

  Exploratory Questions.pdf: outlines the questions that this project addresses

  Data Sources.pdf: outlines the data sources used in this project

  Data Platform.pdf: outlines the overall data architecture and flow for this project

  Project Plan.pdf: a link to the Trello project management plan
  
  Capstone Project Report - Super Finance Bros.pbix: PowerBi dashboard/report for a U.S. Stock Market Analysis
  
  ProjectExecutiveSummary.pdf: Executive Summary covering the background of the stocks we chose to investigate, our methods and technologies used, 
  the results and discussion on our findings, and recommendations based on findings.

### censusData(folder, contents listed below)

  .xls and .xlsx files: raw data from the Census that include historical US total revenue for the given year

  USrevenue.csv: compiled data from the .xls and .xlsx files

## AUTHORS:
yvcvs, dbode777, TKorby, akittendorf
