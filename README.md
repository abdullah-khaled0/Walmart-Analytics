# 📊 Walmart Analytics

![Walmart-Analytics Banner](https://www.supplychainbrain.com/ext/resources/2022/11/15/WALMART-STOREFRONT-iStock-1205217071.jpg?t=1668529933&width=1080)

## Project Overview
This project aims to develop a machine learning solution to predict **weekly retail sales** for a chain of stores, utilizing various external factors such as temperature, fuel prices, CPI (Consumer Price Index), unemployment rates, and holiday flags. Accurate sales forecasting is essential for efficient inventory management, marketing strategies, and optimizing operational processes.

## Dataset Description
The dataset contains historical sales data for multiple stores across different time periods. Below are the main columns included in the dataset:

- **Store**: Unique identifier for each store.
- **Date**: The specific week of the year.
- **Weekly_Sales**: Total sales for the store during that week.
- **Holiday_Flag**: Binary flag indicating whether the week includes a holiday (1) or not (0).
- **Temperature**: The average temperature in the region for that week.
- **Fuel_Price**: Fuel prices in the region during that week.
- **CPI (Consumer Price Index)**: A measure of inflation, affecting consumer purchasing power.
- **Unemployment**: Unemployment rate in the region during that period.

## Project Objective
The objective is to build a robust predictive model that can accurately forecast weekly retail sales based on the provided features. By leveraging historical data and external indicators.

## Methodology
1. **Data Preprocessing**:
   - Handled missing values, removed outliers, and performed log transformations on skewed data.
   - Converted the `Date` column into datetime format and extracted time-based features (optional).
   - Scaled the features using **StandardScaler** for models that require normalized inputs.

2. **Modeling**:
   - Implemented multiple machine learning models to predict weekly sales:
     - **Linear Regression**
     - **Random Forest Regressor**
     - **Gradient Boosting Regressor**
     - **Support Vector Regressor (SVR)**
   - **Random Forest** was chosen as the primary model due to its high performance and ability to capture complex relationships between features.

3. **Evaluation**:
   - Models were evaluated using metrics such as **Mean Absolute Error (MAE)** and **Mean Squared Error (MSE)**.
   - Visualized **Predicted vs. Actual Sales** for a better understanding of model accuracy.
   - Plotted **Feature Importance** to identify which factors most influence weekly sales.

## Results
- The **Random Forest Regressor** performed the best in terms of predictive accuracy, providing reliable estimates of weekly sales.
- **Feature Importance Analysis** revealed that factors like **Fuel_Price**, **CPI**, and **Holiday_Flag** significantly impact sales, helping stores plan more effectively around economic conditions and holidays.

## Installation and Requirements
To run the project, you need the following dependencies installed:

```bash
pip install pandas numpy scikit-learn seaborn matplotlib plotly
