# 🪙 Gold Price Forecasting

This project focuses on forecasting gold prices using classical time series models. The dataset includes historical gold price data, and the objective is to analyze price trends and build predictive models to forecast future values.

---

## 📌 Objective

To predict the future prices of gold based on historical price data using time series forecasting techniques such as:

- Linear Regression
- Naive Forecast
- Exponential Smoothing

---

## 📊 Dataset

- **Source**: [Kaggle – Monthly Gold Price](https://www.kaggle.com/datasets/nhiyen/monthly-gold-price)
- **Duration**: 1950-01 to 2020-07
- **Features**:
  - `Date`: Monthly timestamp
  - `Price`: Gold price in USD
- **Total Records**: 847 observations

---

## 🧠 Models Used

### 1. Linear Regression
- Splits dataset into train and test sets.
- Predicts future prices using a simple linear model.
- Evaluated using Mean Absolute Percentage Error (MAPE).

### 2. Naive Model
- Uses the last observed value as the forecast for all future points.
- Simple baseline model for comparison.

### 3. Exponential Smoothing
- Uses the `statsmodels` package for fitting.
- Accounts for trends and seasonality in the series.
- Produces forecast with 95% confidence intervals.

---

## 📈 Results

- Models were evaluated using **MAPE**.
- **Exponential Smoothing** performed best with a MAPE score of **17.23%**.
- Forecasted gold prices from **2020-08 to 2025-02**.
- Predictions are saved in `gold_price_predictions.csv`.

---

## 🛠️ Tech Stack

- Python 3
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Statsmodels

---