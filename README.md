# USA Domestic Stock Market Analysis 
## PURPOSE:
This is a basic stock market analysis tool created as a capstone project for Dev10. The purpose of this project is to analyze the domestic stock market and its top 5 sectors as determined by market capitalization. Vanguard's top 5 ETF index funds were chosen to represent the top 5 sectors in the US. Vanguard's VTI was chosen as the index fund used to represent the US economy. We compare the historical stock prices of VTI to the total US revenue by year for the years 2006-2020 to validate the latter assumption. Several machine learning models were implemented to see if Vanguard's top 5 ETF index funds were valid indicators of economic trends in the US. This was done by using other US economic features as training and testing data. 

## REQUIREMENTS:
This project utilizes Azure Databricks, Microsoft Azure Data Factories and Pipelines, Kafka Producers and Consumers, SQL databases, and Power BI.

## MAINTENANCE:
This was created for an assignment and will likely not be updated after 2/18/2022.

## REPOSITORY FILES:
[README.md](https://github.com/akittendorf/Domestic-Stock-Market-Analysis#readme)        

[RepeatableETLReport](https://github.com/akittendorf/Domestic-Stock-Market-Analysis/blob/main/RepeatableETLReport.pdf): An ETL document on how to extract, transform, and load data from the Alpha Vantage API into a SQL database

[ProjectExecutiveSummary.pdf](https://github.com/akittendorf/Domestic-Stock-Market-Analysis/blob/main/ProjectExecutiveSummary.pdf): Executive Summary covering the background of the stocks we chose to investigate, our methods and technologies used, 
  the results and discussion on our findings, and recommendations based on findings.

### [Planning](https://github.com/akittendorf/Domestic-Stock-Market-Analysis/tree/main/Planning) (folder, contents listed below):

[DashboardNapkinsAndFeedback.png](https://github.com/akittendorf/Domestic-Stock-Market-Analysis/blob/main/Planning/DashboardNapkinsAndFeedback.pdf): rough sketch of the Power BI dashboard outline

[VisualizationsNapkinsAndFeedback.png](https://github.com/akittendorf/Domestic-Stock-Market-Analysis/blob/main/Planning/VisualizationsNapkinsAndFeedback.pdf): rough sketch of specific visualizations for the Power BI dashboard

[ERD.jpg](https://github.com/akittendorf/Domestic-Stock-Market-Analysis/blob/main/Planning/ERD.jpg): Entity Relationship diagram for how we set-up our SQL database schema


### [Code](https://github.com/akittendorf/Domestic-Stock-Market-Analysis/tree/main/Code) (folder, contents listed below):
  [API-Producer.ipynb](https://github.com/akittendorf/Domestic-Stock-Market-Analysis/blob/main/Code/API-Producer.ipynb): Python code used in Azure Databricks for the Producer of our Azure Data Factory.

  [Base-Consumer.ipynb](https://github.com/akittendorf/Domestic-Stock-Market-Analysis/blob/main/Code/Base-Consumer.ipynb): Python code used in Azure Databricks for the Consumer of our Azure Data Factory.

  [LSTM_Model.ipynb](https://github.com/akittendorf/Domestic-Stock-Market-Analysis/blob/main/Code/LSTM_Model.ipynb): Python Code on how the LSTM model was created and descriptions about the decisions made for key parameters.

  [```Linear Regression Assumptions.ipynb```](https://github.com/akittendorf/Domestic-Stock-Market-Analysis/blob/main/Code/Linear%20Regression%20Assumptions.ipynb): Describes the decisions made about the methodology chosen for the Linear Regression and LassoCV models.

  [```Linear Regression and LassoCV Model for Capstone Project.ipynb```](https://github.com/akittendorf/Domestic-Stock-Market-Analysis/blob/main/Code/Linear%20Regression%20and%20LassoCV%20Model%20for%20Capstone%20Project.ipynb): Python code used to create the Linear Regression and LassoCV models. 

  [Python Visualizations for Power Bi Dashboard.ipynb](https://github.com/akittendorf/Domestic-Stock-Market-Analysis/blob/main/Code/Python%20Visualizations%20for%20Power%20Bi%20Dashboard.ipynb): Contains all Python code used for creating the visualizations in Power BI that used Python scripting (with the exception of the Machine Learning Model comparisons and Historical Price vs. Total US revenue visualizations)

  [arimax.ipynb](https://github.com/akittendorf/Domestic-Stock-Market-Analysis/blob/main/Code/arimax.ipynb): Python code for creating the ARIMA model and descriptions about the decisions made for key parameters.

  [```model comparisons.ipynb```](https://github.com/akittendorf/Domestic-Stock-Market-Analysis/blob/main/Code/model%20comparisons.ipynb): Python code used in constructing the Machine Learning Model Comparison visualization in Power BI.
  
  [Requirements.txt](https://github.com/akittendorf/Domestic-Stock-Market-Analysis/blob/main/Code/requirements.txt): run pip install -r requirements.txt within the same directory to install required modules/libraries.
  
### [```ML Models```](https://github.com/akittendorf/Domestic-Stock-Market-Analysis/tree/main/ML%20Models) (folder, contents listed below):
All machine learning models investigated for this project
  
  [LSTM_ManualSplit_model.h5](https://github.com/akittendorf/Domestic-Stock-Market-Analysis/blob/main/ML%20Models/LSTM_ManualSplit_model.h5)

  [```LassoCV model.model```](https://github.com/akittendorf/Domestic-Stock-Market-Analysis/blob/main/ML%20Models/LassoCV%20model.model)

  [```Linear Regression model.model```](https://github.com/akittendorf/Domestic-Stock-Market-Analysis/blob/main/ML%20Models/Linear%20Regression%20model.model)

  [```SARIMAX joblib.model```](https://github.com/akittendorf/Domestic-Stock-Market-Analysis/blob/main/ML%20Models/SARIMAX%20joblib.model)

  [```arimax model```](https://github.com/akittendorf/Domestic-Stock-Market-Analysis/blob/main/ML%20Models/arimax%20model)

### [```Project Specifications```](https://github.com/akittendorf/Domestic-Stock-Market-Analysis/tree/main/Project%20Specifications) (folder, contents listed below):

  [ExploratoryQuestions.pdf](https://github.com/akittendorf/Domestic-Stock-Market-Analysis/blob/main/Project%20Specifications/ExploratoryQuestions.pdf): outlines the questions that this project addresses

  [```Data Sources.pdf```](https://github.com/akittendorf/Domestic-Stock-Market-Analysis/blob/main/Project%20Specifications/Data%20Sources.pdf): outlines the data sources used in this project

  [```Data Platform.pdf```](https://github.com/akittendorf/Domestic-Stock-Market-Analysis/blob/main/Project%20Specifications/Data%20Platform.pdf): outlines the overall data architecture and flow for this project

  [ProjectManagementPlan.pdf](https://github.com/akittendorf/Domestic-Stock-Market-Analysis/blob/main/Project%20Specifications/ProjectManagementPlan.pdf): a link to the Trello project management plan
  
  [```Capstone Project Report - Super Finance Bros.pbix```](https://github.com/akittendorf/Domestic-Stock-Market-Analysis/blob/main/Project%20Specifications/Capstone%20Project%20Report%20-%20Super%20Finance%20Bros.pbix): PowerBi dashboard/report for a U.S. Stock Market Analysis
  
  [ProjectExecutiveSummary.pdf](https://github.com/akittendorf/Domestic-Stock-Market-Analysis/blob/main/Project%20Specifications/ProjectExecutiveSummary.pdf): Executive Summary covering the background of the stocks we chose to investigate, our methods and technologies used, 
  the results and discussion on our findings, and recommendations based on findings.

### [censusData](https://github.com/akittendorf/Domestic-Stock-Market-Analysis/tree/main/censusData) (folder, contents listed below):

  .xls and .xlsx files: raw data from the Census that include historical US total revenue for the given year

  [USrevenue.csv](https://github.com/akittendorf/Domestic-Stock-Market-Analysis/blob/main/censusData/USrevenue.csv): compiled data from the .xls and .xlsx files

## AUTHORS:
yvcvs, dbode777, TKorby, akittendorf
