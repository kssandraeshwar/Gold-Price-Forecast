# 🟡 Gold Price Forecasting Using Time Series & Machine Learning

This project aims to accurately **predict the future price of gold (GLD)** using a variety of forecasting models, including deep learning (LSTM), machine learning (XGBoost, Random Forest), and statistical approaches (ARIMA, Prophet). The best results were obtained using a **Multivariate LSTM model** incorporating multiple economic indicators.

---

## 📌 Objective

- Forecast gold prices using **time series and machine learning techniques**.
- Compare model performances across univariate and multivariate settings.
- Analyze the influence of features like stock indices, oil prices, silver, and forex on gold.

---

## 📊 Dataset Description

Data is sourced from a historical financial dataset and includes the following features:

| Feature     | Description                                 |
|-------------|---------------------------------------------|
| `Date`      | Date of observation                         |
| `GLD`       | Gold ETF closing price                      |
| `SPX`       | S&P 500 Index                               |
| `USO`       | United States Oil Fund                      |
| `SLV`       | Silver ETF                                  |
| `EUR/USD`   | Euro to US Dollar exchange rate             |

---

## 🔍 Models Implemented

| Model Type          | Model Used           | Input Type        |
|---------------------|----------------------|-------------------|
| ✅ Deep Learning     | LSTM (Univariate)    | Only GLD          |
| ✅ Deep Learning     | **Multivariate LSTM**| All features      |
| 🔁 Statistical       | ARIMA                | GLD               |
| 🔁 Statistical       | Prophet              | GLD               |
| 🤖 Machine Learning  | XGBoost Regressor    | All features      |
| 🤖 Machine Learning  | Random Forest        | All features      |

---

## ✅ Model Evaluation

| Model             | RMSE     | MAE      |
|------------------|----------|----------|
| LSTM (Univariate) | Moderate | Moderate |
| **LSTM (Multivariate)** | ✅ **Low**   | ✅ **Low**   |
| ARIMA             | Moderate | Moderate |
| Prophet           | Moderate | Moderate |
| XGBoost           | Good     | Good     |
| Random Forest     | Good     | Good     |

> The **Multivariate LSTM** performed best in terms of RMSE and MAE.

---

## 📈 Visual Output

- Actual vs Predicted Gold Prices (LSTM & Others)
- Loss Curves (Training vs Validation)
- Feature Correlation Heatmap
- Time Series Line Plots

---

## 🔧 Tech Stack

- Python
- Pandas, NumPy, Scikit-Learn
- TensorFlow / Keras
- XGBoost
- Facebook Prophet
- Matplotlib / Seaborn

---

## 📦 How to Run

1. Clone this repo
2. Open the Colab notebook: `Gold_Price_Forecast.ipynb`
3. Run cells step-by-step (install libraries if required)
4. Compare results and visualize outputs

---

## 📌 Future Work

- Hyperparameter tuning for LSTM & XGBoost
- Incorporate more macroeconomic indicators
- Real-time prediction dashboard using Streamlit

---


