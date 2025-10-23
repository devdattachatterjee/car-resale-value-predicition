# 🚗 Used Car Price Prediction: Regression Analysis

## 🎯 Project Goal
The primary objective of this project was to develop a highly accurate machine learning model to estimate the resale price of a used car. This accuracy is vital for used-car marketplaces to optimize pricing strategies, maximize seller conversions, and increase profit margins.

## ⚙️ Methodology & Pipeline
The project followed a standard Machine Learning pipeline, focusing on transforming skewed price data into a robust format for analysis:

1.  **Data Preparation:**
    * **Feature Engineering:** Created the key variable **`Car_Age`** (Current Year - Year) to quantify depreciation.
    * **Normalization:** Applied **Log Transformation** to the `Selling_Price` target variable to correct severe right-skewness and stabilize model variance.
2.  **Exploratory Data Analysis (EDA):** Confirmed the strong influence of price factors and checked data quality after transformation.
3.  **Modeling & Evaluation:** Trained and compared three regression models to determine the optimal approach for the market data.

## ✨ Key Results & Model Performance

| Model | R² Score | MAE (Mean Absolute Error) |
| :--- | :--- | :--- |
| **Random Forest (Winner)** | **~0.95** | **~0.50 Lakhs (₹50,000)** |
| Linear Regression (Baseline) | ~0.88 | ~0.85 Lakhs (₹85,000) |
| Decision Tree | ~0.93 | ~0.60 Lakhs (₹60,000) |

The **Random Forest Regressor** proved superior by capturing non-linear relationships, achieving a final accuracy where the average prediction error was only about **₹50,000**.

## 💡 Business Insights (Key Findings)

The model's **Feature Importance** (which you visualized) provided critical market insights:

1.  **Dominant Factor:** The **`Present_Price`** (the current showroom value) accounts for the vast majority of the price prediction power.
2.  **Depreciation:** **`Car_Age`** is the second most important feature, directly quantifying the economic concept of value loss over time.
3.  **Value Retention:** Diesel cars and cars with Automatic transmission consistently show a higher median log price (and thus a higher resale value) than their Petrol and Manual counterparts.

---
### Top 5 Predictors (Feature Importance)
