

#  Gold Price Forecasting Using Time Series & Machine Learning

This project aims to accurately predict the future price of gold (GLD) using a variety of forecasting models, including deep learning (LSTM), machine learning (XGBoost, Random Forest), and statistical approaches (ARIMA, Prophet). The best results were achieved using a **Multivariate LSTM model** that incorporates various economic indicators.

---

##  Objective

* Forecast gold prices using time series and machine learning techniques
* Compare model performances across univariate and multivariate settings
* Analyze the influence of external features such as stock indices, oil prices, silver, and forex rates on gold

---

##  Dataset Description

Historical financial data including:

| Feature | Description                     |
| ------- | ------------------------------- |
| Date    | Date of observation             |
| GLD     | Gold ETF closing price          |
| SPX     | S\&P 500 Index                  |
| USO     | United States Oil Fund          |
| SLV     | Silver ETF                      |
| EUR/USD | Euro to US Dollar exchange rate |

---

##  Models Implemented

| Model Type          | Model Used          | Input Type   |
| ------------------- | ------------------- | ------------ |
| ✅ Deep Learning     | LSTM (Univariate)   | Only GLD     |
| ✅ Deep Learning     | LSTM (Multivariate) | All features |
| 🔁 Statistical      | ARIMA               | GLD          |
| 🔁 Statistical      | Prophet             | GLD          |
| 🤖 Machine Learning | XGBoost Regressor   | All features |
| 🤖 Machine Learning | Random Forest       | All features |

---

##  Model Evaluation

| Model               | RMSE     | MAE      |
| ------------------- | -------- | -------- |
| LSTM (Univariate)   | Moderate | Moderate |
| LSTM (Multivariate) | ✅ Low    | ✅ Low    |
| ARIMA               | Moderate | Moderate |
| Prophet             | Moderate | Moderate |
| XGBoost             | Good     | Good     |
| Random Forest       | Good     | Good     |

 **Multivariate LSTM gave the best performance** with the lowest RMSE and MAE.

---

##  Visual Outputs

* ✅ Actual vs. Predicted Gold Prices (across all models)
* ✅ Loss Curves (Training vs. Validation for LSTM)
* ✅ Forecasting Graphs (Prophet, ARIMA, etc.)
* ✅ Time Series Line Plots (GLD, SPX, USO, etc.)

---

##  Tech Stack

* **Language**: Python
* **Libraries**:

  * Pandas, NumPy
  * Scikit-Learn
  * TensorFlow / Keras
  * XGBoost
  * Facebook Prophet
  * Matplotlib, Seaborn

---

Let me know if you’d like this saved as a Markdown file or need a version with embedded visuals.
