
# Sales Forecast Model

This project focuses on developing a machine learning model to predict monthly sales by segment for retailers in shopping malls. The model was built using a Decision Tree Regressor, optimized for the best negative mean absolute error (neg_mean_absolute_error). Key steps in the project include data collection, cleaning, exploratory data analysis, outlier detection, and stationarity testing using KPSS, ADF, OCSB, and CH tests. The model was fine-tuned using hyperparameter optimization and evaluated with metrics such as MSE, MAE, and R². The final model predicts an 3% increase in total sales over the next 12 months compared to the previous year, providing valuable insights for strategic decision-making.

![aaaaa](https://github.com/filipegoncmartins/Customer-Segmentation-Analysis-using-Machine-Learning/assets/148718210/e95d2a59-0849-47a0-82bc-5a2b2724e5ab)


## Problem to be Solved

The problem addressed in this project is the need for accurate and reliable forecasts of monthly sales for different store segments within shopping malls. Retailers and mall management require these predictions to make informed decisions about inventory management, marketing strategies, and resource allocation. The challenge lies in developing a model that can account for the diverse factors affecting sales, including seasonal trends and segment-specific behaviors, while providing precise forecasts that can guide strategic planning and optimize business operations.

## Dataset Information

The dataset used in this project was extracted from an internal data warehouse and exported to Excel for analysis. It contains comprehensive information relevant to the sales performance of different store segments within shopping malls. The dataset includes the following columns: Mall, Cod_client, Sales, Categoria (Category), Segmento (Segment), Tipo de Locação (Lease Type), Classificação (Classification), Data (Date), Ano (Year), and Mês (Month). This data provides a detailed view of sales across various segments between 2018 and 2024, serving as the foundation for building and evaluating the predictive model.

## Steps followed 

### [1]  Data Collection and Cleaning

* Gather relevant data, such as sales records and store attributes. Integrate these datasets into a unified dataset.
* Clean the data by removing duplicates and correcting inconsistencies.
* Identify and handle missing values through imputation or removal as needed.

### [2]  Exploratory Data Analysis (EDA)
* Inspect the dataset to identify patterns, trends, and potential anomalies.
* Use visualizations like histograms and time series plots to understand data distributions and behavior.
* Analyze sales by different store segments.
### [3]  Outlier Detection
* Decide on appropriate treatment for outliers, whether by removal, transformation, or imputation.
### [4]  Stationarity Tests
* Perform tests such as KPSS, ADF, OCSB, and CH to check for stationarity, a key requirement for many time series models.
### [5]  Label Encoding
* Convert categorical variables into numerical labels to make them suitable for machine learning models.
### [6]  Correlation Analysis
* Calculate correlations between variables to understand their relationships and identify potential multicollinearity issues.
### [7]  Model Selection with Cross-Validation
* Evaluate different models (Ridge, Lasso, RandomForestRegressor, DecisionTreeRegressor, KNeighborsRegressor) using cross-validation, optimizing performance based on negative mean absolute error (neg_mean_absolute_error).
### [8]  Hyperparameter Tuning with GridSearchCV
* Use GridSearchCV to search for the best parameters for the selected model, improving its performance.
### [9]  Model Evaluation
* Assess model accuracy and performance using metrics like MSE, MAE, and R².
### [10]  Precision for 12-Month Forecast
* Verify the model's precision over a 12-month prediction horizon and adjust as necessary to ensure reliable forecasts.

## Insights

* Segmented Sales Trends: The model revealed distinct sales patterns across different store segments, allowing for more targeted analysis and decision-making. Retail segments responded differently to seasonal variations, highlighting the importance of segment-specific strategies.

* Stationarity Confirmation: The time series data was confirmed to be stationary through multiple tests (KPSS, ADF, OCSB, and CH), ensuring the reliability of the forecasting model without the need for further transformations.

* Model Accuracy: The Decision Tree Regressor model, optimized for the best negative mean absolute error, demonstrated high accuracy with an R² score of 0.971. This indicates a strong fit to the historical data and a reliable prediction capability.

* 12-Month Sales Forecast: The model predicts an 3% increase in total sales over the next 12 months compared to the previous period. This forecast provides actionable insights for inventory management, marketing strategies, and resource allocation.

* Impact of Excluding Pandemic Data: By removing the months corresponding to the peak of the pandemic from the dataset, the model was better able to capture typical sales patterns, leading to more accurate and relevant forecasts for future periods.

These insights support strategic decision-making by providing a deeper understanding of sales dynamics across different store segments and time periods within the shopping malls.

## Conclusion

In conclusion, this project successfully developed a robust machine learning model for forecasting monthly sales by segment within shopping malls. By leveraging a Decision Tree Regressor and optimizing its performance through meticulous data preparation and model tuning, we achieved a highly accurate forecast with an impressive R² score of 0.971. 

The model’s prediction of an 3% increase in sales over the next 12 months offers valuable foresight for strategic planning, enabling retailers and mall management to make informed decisions regarding inventory, marketing, and resource allocation. 

The thoughtful exclusion of pandemic-related anomalies further refined the model, ensuring that the forecasts reflect more typical business conditions. Overall, this project not only enhances our understanding of sales trends across different segments but also equips stakeholders with actionable insights to drive future success.
