# 🛢️ WTI Price Prediction

This project uses **machine learning** to predict the **WTI crude oil index** based on historical WTI prices and the NYSE Index.  
It collects real-world financial data from Yahoo Finance, stores it in a **MySQL database**, and then trains a simple **Decision Tree Classifier** to make predictions.

---

## 📊 Project Overview

The project consists of two main scripts:

### 1. `fetch_data.py`
- Scrapes historical data from Yahoo Finance:
  - `date`
  - `WTI_Price`
  - `NYSE_Index`
  - `WTI_Index`
- Stores all data in a MySQL table named **Oil**.

### 2. `machine_Learning.py`
- Loads the data from MySQL.
- Trains a **Decision Tree Classifier** using scikit-learn.
- Takes two inputs from the user:
  - The considered Oil Barrel Price
  - The considered NYSE Index
- Predicts the approximate **WTI Index**.

---

## ⚙️ Requirements

Make sure the following dependencies are installed:

```bash
pip install mysql-connector-python requests beautifulsoup4 scikit-learn
