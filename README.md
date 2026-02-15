# 📈 Stock Price Prediction Web App  
### Machine Learning-Based Next-Day Opening Price Forecast

## 📌 Project Overview

This project predicts the **next day’s opening stock price** based on historical stock data using **Lasso Regression**.

The application dynamically:

1. Fetches historical stock data using `yfinance`
2. Cleans and preprocesses the dataset
3. Trains a regression model on the selected stock
4. Predicts tomorrow’s opening price using today’s closing price
5. Displays the result through a web interface

The model was deployed using **Flask** on the **PythonAnywhere** platform (deployment no longer active).

---

## 🎯 Objective

To build an end-to-end machine learning application that:

- Retrieves real-time financial data
- Performs preprocessing and feature analysis
- Trains a regression model
- Generates stock price predictions
- Serves predictions via a web interface

---

## 🔍 Data Pipeline

### 1️⃣ Data Collection
- Historical stock data fetched using the `yfinance` API
- Data retrieved dynamically based on user-entered stock ticker

Example:
User enters: AAPL
System fetches: AAPL historical price data


---

### 2️⃣ Data Cleaning & Preparation

The dataset was processed to:

- Remove missing values
- Ensure proper datetime indexing
- Extract relevant price features
- Align today's closing price with tomorrow's opening price (target shift)

Target formulation:

Feature → Today's Close Price
Target → Tomorrow's Open Price

This converts time series data into a supervised regression problem.

---

## 🧠 Model Used

### 🔵 Lasso Regression

Lasso Regression (L1 regularization) was selected to:

- Reduce overfitting
- Penalize unnecessary feature weights
- Improve generalization

The model is trained dynamically after a stock ticker is entered.

This means:
- Each stock symbol has its own trained model
- The model learns patterns specific to that stock’s historical behavior

---

## 🔄 Prediction Flow

1. User enters stock ticker
2. App fetches historical data
3. Data is cleaned and prepared
4. Lasso model is trained
5. Model predicts tomorrow's opening price based on today's closing price
6. Result is displayed in the web interface

---

## 🌐 Deployment

- Built using **Flask**
- Deployed on **PythonAnywhere**
- Web-based user interface for interaction

⚠️ Deployment is currently inactive, but the full application code remains in this repository.

---

## 🛠 Tech Stack

- Python  
- Flask  
- scikit-learn  
- yfinance  
- Pandas  
- NumPy  
- HTML/CSS  

---

## 📂 Project Structure


This converts time series data into a supervised regression problem.

---

## 🧠 Model Used

### 🔵 Lasso Regression

Lasso Regression (L1 regularization) was selected to:

- Reduce overfitting
- Penalize unnecessary feature weights
- Improve generalization

The model is trained dynamically after a stock ticker is entered.

This means:
- Each stock symbol has its own trained model
- The model learns patterns specific to that stock’s historical behavior

---

## 🔄 Prediction Flow

1. User enters stock ticker
2. App fetches historical data
3. Data is cleaned and prepared
4. Lasso model is trained
5. Model predicts tomorrow's opening price based on today's closing price
6. Result is displayed in the web interface

---

## 🌐 Deployment

- Built using **Flask**
- Deployed on **PythonAnywhere**
- Web-based user interface for interaction

⚠️ Deployment is currently inactive, but the full application code remains in this repository.

---

## 🛠 Tech Stack

- Python  
- Flask  
- scikit-learn  
- yfinance  
- Pandas  
- NumPy  
- HTML/CSS  

---

## 📂 Project Structure


This converts time series data into a supervised regression problem.

---

## 🧠 Model Used

### 🔵 Lasso Regression

Lasso Regression (L1 regularization) was selected to:

- Reduce overfitting
- Penalize unnecessary feature weights
- Improve generalization

The model is trained dynamically after a stock ticker is entered.

This means:
- Each stock symbol has its own trained model
- The model learns patterns specific to that stock’s historical behavior

---

## 🔄 Prediction Flow

1. User enters stock ticker
2. App fetches historical data
3. Data is cleaned and prepared
4. Lasso model is trained
5. Model predicts tomorrow's opening price based on today's closing price
6. Result is displayed in the web interface

---

## 🌐 Deployment

- Built using **Flask**
- Deployed on **PythonAnywhere**
- Web-based user interface for interaction

⚠️ Deployment is currently inactive, but the full application code remains in this repository.

---

## 🛠 Tech Stack

- Python  
- Flask  
- scikit-learn  
- yfinance  
- Pandas  
- NumPy  
- HTML/CSS  

---

## 📂 Project Structure
Stock-Price-Prediction/
│
├── app.py
├── single.py
├── templates/
├── static/
├── requirements.txt
└── README.md

---

## 📊 Key Concepts Demonstrated

- Financial time series handling  
- Feature-target shifting  
- Regularized regression (Lasso)  
- Dynamic model training  
- Web deployment of ML models  
- End-to-end ML pipeline development  

---

## 🚀 How to Run Locally


bash
git clone https://github.com/sksalman0/Stock-Price-Prediction.git
cd Stock-Price-Prediction
pip install -r requirements.txt
python app.py
Then open:http://127.0.0.1:5000/


SK Salman
Aspiring Data Analyst | Machine Learning Enthusiast
