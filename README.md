## 🧠 Introduction

Stock market prices are dynamic and influenced by multiple factors. Predicting these prices accurately is a challenging but insightful task.
In this project, we use **deep learning**, specifically a **SimpleRNN model**, to learn from past price trends and predict future stock values of Apple (AAPL).
The model demonstrates how recurrent architectures can capture sequential dependencies in time-series financial data.

---

## 📊 Dataset

* **Stock Data Source:** [Yahoo Finance (AAPL)](https://finance.yahoo.com/quote/AAPL/)
* **Time Period:** 2020-01-01 to 2025-01-01
* **Feature Used:** Closing Price

---

## ⚙️ Technologies Used

* **Python**
* **TensorFlow / Keras**
* **NumPy**
* **Pandas**
* **Matplotlib**
* **Scikit-learn**
* **Yahoo Finance (yfinance)**

---

## 🧩 Model Architecture

The model consists of:

* **Two SimpleRNN layers** with 50 units each
* **One Dense layer** for output
* **Adam optimizer** and **Mean Squared Error (MSE)** loss function

Training was done on 80% of the dataset with a **time step of 60 days** and **20 epochs**.

---

## 📈 Results

| Metric   | Value   |
| -------- | ------- |
| **MSE**  | 0.00038 |
| **RMSE** | 3.79    |
| **MAE**  | 2.75    |

The model successfully followed the real stock trend with minor lag and smoothing, typical for RNN-based predictions.

**Visualization:**
The blue line represents the real stock price, and the red line represents the predicted price.

![AAPL Prediction](722106e5-4fb1-4ba8-9d2c-476036f28c60.png)


## 📚 Conclusion

This project demonstrates how RNNs can effectively model and predict stock market trends based on historical data.
While the predictions capture general trends, real-world forecasting remains complex due to volatility and external factors.
Future improvements with advanced models and additional features can enhance accuracy and reliability.
