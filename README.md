# 📈 BitPredict: Bitcoin Price Forecasting using Deep Learning

## 🚀 Overview
BitPredict is a deep learning-based time series forecasting project that predicts future Bitcoin prices using historical data.

This project explores multiple machine learning and deep learning architectures implemented in TensorFlow to model and forecast cryptocurrency price trends.

> ⚠️ Disclaimer: This project is for educational and research purposes only. Cryptocurrency markets are highly volatile, and accurate prediction is extremely challenging.

---

## 🎯 Objective
The main goal of this project is to:
- Understand time series forecasting techniques
- Apply deep learning models to financial data
- Compare different architectures for prediction accuracy
- Analyze how well models capture patterns in Bitcoin price movements

---

## 📊 What is Time Series Forecasting?
A time series is a sequence of data points collected over time.  
In this project:

- **Input:** Historical Bitcoin prices  
- **Output:** Future Bitcoin price  

This is a **forecasting problem** (predicting continuous values).

---

## 📂 Dataset
- Source: Yahoo Finance (via `yfinance`)
- Asset: **BTC-USD**
- Time Range: **October 2013 – December 2025**
- Features Used:
  - Date
  - Closing Price (USD)

---

## 🛠️ Tech Stack
- **Python**
- **TensorFlow / Keras**
- **NumPy**
- **Pandas**
- **Matplotlib**
- **yFinance**

---

## ⚙️ Project Workflow

### 1. Data Collection
- Downloaded historical Bitcoin data using `yfinance`
- Stored dataset in CSV format

### 2. Data Preprocessing
- Converted date column to datetime
- Selected closing price as primary feature
- Handled missing values

### 3. Time Series Preparation
- Converted data into supervised learning format (windowing)
- Created:
  - **Univariate dataset**
  - **Multivariate dataset (later stage)**

### 4. Train-Test Split
- Used **chronological split** (NOT random)
  - 80% Training
  - 20% Testing

### 5. Model Building
Implemented multiple models:

| Model No. | Model Type |
|----------|------------|
| 0 | Naïve Baseline |
| 1 | Dense Neural Network |
| 2 | Dense (larger window) |
| 3 | Multi-step Dense |
| 4 | CNN (Conv1D) |
| 5 | LSTM |
| 6 | Multivariate Dense |
| 7 | N-BEATS |
| 8 | Ensemble Model |
| 9 | Future Forecast Model |
| 10 | Data Shift Simulation Model |

---

## 🧠 Key Concepts

### 🔹 Window
Number of past time steps used as input  
Example: Last 7 days

### 🔹 Horizon
Number of future steps predicted  
Example: Next 1 day

---

## 📈 Baseline Model (Naïve Forecast)
The simplest model used:
ŷ(t) = y(t-1)

- Uses previous value as prediction
- Serves as a benchmark for comparison

---

## 📏 Evaluation Metrics

### Scale-dependent metrics:
- MAE (Mean Absolute Error)
- RMSE (Root Mean Squared Error)

### Percentage-based metrics:
- MAPE (Mean Absolute Percentage Error)

Lower values indicate better performance.

---

## 📊 Results & Insights
- Naïve model performs surprisingly well (strong baseline)
- Deep learning models capture trends but struggle with volatility
- LSTM and CNN improve temporal understanding
- Ensemble models provide more stable predictions

---

## 🔮 Applications
Time series forecasting is widely used in:
- 📈 Financial markets
- 🛒 Sales forecasting
- ⚡ Energy consumption prediction
- 🌦️ Weather forecasting

---

## 📌 Future Improvements
- Add real-time prediction using APIs
- Deploy model using Flask / FastAPI
- Integrate with a web dashboard
= Improve accuracy using transformers
- 🤝 Contributing

---

## 👨‍💻 Author
**Subhankar Pandit**  
**Full Stack Developer | Backend Engineer | AI/ML | Cloud**  
**GitHub**: https://github.com/SubhankarA8415  
**LinkedIn**: https://linkedin.com/in/subhankar-pandit 

---

## 📜 License
**This project is licensed under the MIT License.**
