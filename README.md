# PredictiveAnalysis: Loan Portfolio
An analysis predicting the amount to be disbursed in loans 

Project Overview
This project is focused on analyzing and visualizing loan portfolio data, with an emphasis on understanding customer behavior across various sectors, products, and classifications. Additionally, time series predictive modeling techniques were implemented to forecast loan disbursements over time, which can assist in financial planning and risk assessment.

Key Objectives
- Conduct exploratory data analysis on loan disbursements, outstanding amounts, and arrears.
- Visualize trends in loan disbursements by sector, product, and customer demographics.
- Build predictive models to forecast future loan disbursements using time series analysis.
Project Structure: This project is divided into two main parts:

Exploratory Data Analysis (EDA):
- Performed various analyses to gain insights into the loan portfolio, including loan disbursement trends, outstanding loan amounts by product, and customer segmentation by sector.
Key visualizations include:
- Loan distribution by gender, loan type, and classification.
- Top 20 products by total outstanding loan amounts.
- Average loans disbursed by sector and product.
Predictive Modeling:
- Developed time series models to predict future loan disbursements, which help estimate the expected cash flow for upcoming periods.
Models used include:
- Linear Regression: Utilized lagged variables for a simple predictive model.
- AutoRegressive (AR) model: Implemented for enhanced temporal forecasting accuracy with rolling and walk-forward validation.
Code Walkthrough:
-- Exploratory Data Analysis (EDA)
Data Filtering and Cleaning: Cleaned and transformed the dataset, including data replacements and aggregations.
Sector and Product Analysis: Grouped data by sector and product to observe the highest concentrations of loans.
Classification Analysis: Regularized loan classifications to identify trends across loan statuses (e.g., Performing, Doubtful, Lost).
Loan Distribution: Visualized loan counts by gender and loan type.
-- Predictive Modeling
Time Series Preparation: Aggregated and resampled the data for daily, weekly, and monthly loan disbursement tracking.
Model Selection: Developed and tested models on train-test splits, incorporating metrics such as Mean Absolute Error (MAE).
Linear Regression: Implemented a simple linear regression model using previous day’s disbursement as a lagged feature.
AutoRegressive (AR): Built an AR model with optimal lag settings and conducted walk-forward validation for real-time prediction adjustment.


Results
Exploratory Analysis Insights:
Identified sectors with the highest loan disbursement and arrears to aid in risk management.
Showcased classification distribution for better portfolio quality assessment.
Predictive Model Performance:
Achieved reasonable accuracy with the AR model and validated the model’s MAE on both training and test datasets.
Developed insights from the walk-forward validation, showcasing the AR model’s adaptability to changing data patterns.


Conclusion and Recommendations based on the analyses and predictions:
Loan Concentration: Sectors and products with high disbursement (e.g SME loans) or outstanding amounts may need closer monitoring for risk management.
Predictive Insights: Time series predictions of disbursements provide valuable insights into future cash flow, aiding financial planning.


Dependencies
Python packages: pandas, matplotlib, seaborn, scikit-learn, statsmodels, plotly

