
# Sales Forecast Model

This repository contains a sales forecast model developed for a retail store using Python. The model predicts the quantity of sales for the next four weeks, utilizing historical sales data and various other factors.

![aaaaa](https://github.com/filipegoncmartins/Customer-Segmentation-Analysis-using-Machine-Learning/assets/148718210/e95d2a59-0849-47a0-82bc-5a2b2724e5ab)


## Problem to be Solved

The objective of this project is to forecast the weekly sales quantities for the Back Bay store, using sales data from this store as well as from other stores in the network. By doing so, the model helps in planning and decision-making processes, ensuring that the store can meet customer demand efficiently.

## Dataset Information

This project utilizes three primary datasets to build the sales forecast model:

* Calendar Data (dfcalendar)
The calendar dataset provides information on dates, including the day of the week and any special events. This data is crucial for capturing seasonal patterns and event-driven sales spikes. It includes fields for the date, the corresponding weekday in both string and integer formats, and event names when applicable.

* Price Data (dfprice)
The price dataset contains detailed pricing information for items sold across various stores. It includes the item identifier, its category, the store code, the specific week of the year, and the selling price. This dataset helps in understanding how price changes affect sales volumes, allowing the model to account for price sensitivity.

* Sales Data (dfsales)
The sales dataset is the most extensive and contains transaction-level details for each item sold. It includes fields such as the item ID, item category, department, store name, store code, region, the day of the sale, and the sales quantity. This dataset is essential for training the model as it provides the historical sales data needed to identify patterns and trends.

## Steps followed 

### [1]  Data Preprocessing
Standard procedures for data analysis were followed, including: 

* Cleaning the data to handle missing values and inconsistencies.
* Transforming the data to ensure compatibility with modeling techniques.
* Feature engineering to create relevant features for the model.

### [2]  Model Selection

Various models were evaluated using cross-validation to ensure robust performance. Ridge Regression was identified as the best-performing model.

### [3]  Forecasting

Sales data were aggregated weekly. The forecast for the Back Bay store was made using sales data from both the Back Bay store and other stores in the network.

### [4]  Optimization

A model optimization algorithm was employed to fine-tune the Ridge Regression model for better accuracy.

## Insights

* Seasonal Trends: Analysis revealed significant seasonal trends that impact sales, which were incorporated into the model.
* Price Sensitivity: Sales showed sensitivity to changes in prices, underlining the importance of including price data in the model.
* Event Impact: Events listed in the dfcalendar dataset had notable effects on sales, demonstrating the need to account for external factors.

## Conclusion

The final Ridge Regression model successfully projected sales quantities for the next four weeks for the Back Bay store. The model's predictions can aid in inventory management and strategic planning.
