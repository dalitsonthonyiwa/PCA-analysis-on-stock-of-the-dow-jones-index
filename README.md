# 📊 PCA on a Stock Portfolio (Dow Jones 30)

This project applies **Principal Component Analysis (PCA)** to a portfolio of **Dow Jones Industrial Average (DJIA) stocks** to analyze correlations, reduce dimensionality, and identify the main drivers of market movement.

The notebook retrieves historical stock price data, preprocesses it, performs PCA, and visualizes both variance explained and correlation structures within the portfolio.

---

## 🚀 Project Overview

Financial markets often contain highly correlated assets. This project demonstrates how **PCA** can be used to:

- Reduce redundancy in correlated stock returns  
- Identify dominant market factors  
- Understand the structure of a diversified stock portfolio  
- Support exploratory analysis for portfolio construction  

---

## 📂 Data Source

- **Stock data** is downloaded directly from **Yahoo Finance** using the `yfinance` library  
- **Assets**: Dow Jones 30 stocks  
- **Time period**: From **January 1, 2020** onward  
- **Price used**: Adjusted closing prices  

---

## 🧪 Methodology

### 1. Data Collection
- Fetch daily closing prices for all Dow Jones 30 stocks
- Rename tickers to company names for improved readability

### 2. Data Preprocessing
- Convert prices to **daily returns**
- Handle missing values
- Standardize features using **StandardScaler**

### 3. Principal Component Analysis (PCA)
- Apply PCA to standardized returns
- Analyze:
  - Explained variance ratio
  - Cumulative explained variance
- Identify stocks with the highest contributions to the leading principal components

### 4. Correlation Analysis
- Compute absolute correlation matrix
- Identify highly correlated stocks (correlation > 0.9)
- Remove redundant assets
- Visualize correlation matrices **before and after filtering**

---

## 📈 Visualizations Included

- Time-series plot of stock returns  
- PCA explained variance bar chart  
- Cumulative explained variance plot  
- Correlation heatmaps:
  - Full Dow Jones portfolio  
  - Reduced (less correlated) portfolio  

---

## 🛠️ Technologies & Libraries

- Python  
- yfinance  
- pandas  
- numpy  
- scikit-learn  
- matplotlib  
- seaborn  

---

