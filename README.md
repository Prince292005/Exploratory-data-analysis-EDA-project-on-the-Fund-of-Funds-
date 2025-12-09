# Exploratory data analysis(EDA) project on the Fund of Funds 
 This project analyzes 10 years of Fund of Funds (FoF) NAV data to study long‑term trends, compare Domestic and Overseas fund performance, and evaluate risk, volatility, and stability. Through detailed data cleaning, visualization, and feature engineering, the project identifies key behavioural patterns in FoFs. A 30-day LSTM time-series model is used to capture sequential NAV movements and generate accurate 14-day forecasts. Overall, the project provides a comprehensive data-driven pipeline from analysis to prediction, offering clear insights into FoF performance and future NAV behaviour.

---

# 📊 Fund of Funds (FoF) NAV Analysis & 14‑Day Forecasting using LSTM

-This project focuses on analyzing **10 years of NAV data** of multiple **Fund of Funds (FoF)** schemes and forecasting the next **14 days of NAV values** using an **LSTM deep learning model**.  
-The project compares **Domestic vs Overseas FoFs**, studies risk–return behaviour, creates financial features, and visualizes trends for meaningful insights.

---

## 🚀 Project Objectives
- Analyze long‑term NAV behaviour of Funds of Funds  
- Study Domestic vs Overseas category performance  
- Engineer risk‑based and return‑based features  
- Visualize NAV trends, volatility, stability & correlations  
- Build an LSTM model for 14‑day NAV forecasting  
- Understand risk, stability, and market behaviour through data  

---

## 📁 Dataset
- **10+ years of NAV data**  
- Contains: `date`, `fund name`, `NAV`, `fund type`, calculated metrics  
- Cleaned, sorted, and processed for time‑series analysis

---

## 🧹 Data Preprocessing
- Converted date to datetime format  
- Sorted dataset chronologically  
- Removed missing or duplicate entries  
- Normalized NAV values using **MinMaxScaler (0–1)**  
- Created **30‑day sliding windows** for LSTM input  

---

## 📊 Exploratory Data Analysis (EDA)

### 🔹 **Univariate Analysis**
- Long‑term NAV trends  
- Volatility distribution  
- Daily return distribution  
- Stability score distribution  

### 🔹 **Bivariate Analysis**
- Volatility vs Stability  
- NAV vs Returns  
- Category vs Volatility (Domestic vs Overseas)  

### 🔹 **Multivariate Analysis**
- Correlation heatmap of daily returns  
- Risk–return–stability comparison  
- Rolling statistics (mean, variance, volatility)

---

## 🧠 Feature Engineering
Created financial indicators such as:
- **Daily Returns**
- **Rolling Returns**
- **Annualized Volatility**
- **Maximum Drawdown**
- **Sharpe‑like Ratio**
- **Stability Score**
- **Rolling Mean & Rolling Std**

These features helped interpret FoF behaviour and prepare the model for forecasting.

---

## 🤖 LSTM Model Architecture
- Input: 30‑day NAV sequence  
- LSTM Layer 1: 50 units  
- LSTM Layer 2: 50 units  
- Dropout Layer: 20%  
- Dense Output Layer: 1 (Next‑day NAV)  

**Optimizer:** Adam  
**Loss:** Mean Squared Error  
**Epochs:** 20  

---

## 🔮 Forecasting Method
- Autoregressive multi‑step approach  
- Predict next day → append → predict next → repeat for 14 days  
- Produces smooth and realistic NAV forecasts  

---

## 🏁 Results
- Model successfully follows real NAV trend  
- Domestic FoFs show higher stability & lower volatility  
- Overseas FoFs show higher fluctuations  
- Forecast curve aligns closely with actual NAV behaviour  
- Heatmaps, risk metrics, and distributions reveal clear category differences  

---

## 📝 Conclusion
The project effectively demonstrates how FoFs behave in terms of risk, stability, and return.  
Using LSTM for time‑series forecasting provides accurate short‑term predictions.  
Feature engineering and EDA helped uncover important insights about fund behaviour.

---

## 🔮 Future Scope
- Extend forecasting to 30‑day or 60‑day periods  
- Add global indicators (gold price, USD‑INR, S&P 500, inflation)  
- Build a web dashboard for real‑time NAV prediction  
- Experiment with advanced models (GRU, Transformer, CNN‑LSTM)  

---

## 🛠️ Technologies Used
- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit‑Learn  
- TensorFlow / Keras  
- Time‑Series Forecasting  

---

## 👨‍💻 Group members

- **Jenish vasani**
- **Prince Sojitra**  
- **Siddharth Vala**  


---
