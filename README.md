# Arch Technologies — Data Science Internship

**Intern:** Maryam Muzammil  
**Program:** Data Science Internship  
**Organization:** Arch Technologies  

---

## Overview

This repository contains 2 tasks completed as part of the Data Science Internship at Arch Technologies. Both tasks involve real-world datasets, data preprocessing, machine learning model building, and performance evaluation.

**Tools & Libraries:** Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, YFinance

---

## Task 1: Titanic Survival Classification

**Objective:**
Predict whether a passenger survived the Titanic disaster based on features like age, gender, ticket class, and fare.

**Dataset:** Titanic Dataset (loaded via Seaborn)

**Approach:**
- Loaded and inspected the Titanic dataset
- Handled missing values — filled age with median, embarked with mode
- Engineered new features: family size, encoded gender and embarkation port
- Trained and compared Decision Tree and Random Forest classifiers
- Evaluated using accuracy score, classification report, confusion matrix, and ROC curve

**Results & Insights:**
- Gender was the most influential factor — women had a much higher survival rate
- 1st class passengers survived at a significantly higher rate than 3rd class
- Passengers traveling alone had lower survival chances than those with family
- Random Forest outperformed Decision Tree with better accuracy and ROC-AUC score

---

## Task 2: Stock Price Prediction

**Objective:**
Predict future stock closing prices based on historical data including open, high, low, close, and volume.

**Dataset:** Apple Inc. (AAPL) stock data fetched via YFinance (2019–2024)

**Approach:**
- Downloaded real-time historical stock data using the `yfinance` library
- Engineered lag features: previous day close, open, high, low, volume
- Added price change and high-low range as additional features
- Trained and compared Linear Regression and Random Forest Regressor
- Evaluated using MAE, RMSE, and R2 Score

**Results & Insights:**
- Previous day closing price is the strongest predictor of next day's price
- Random Forest captured non-linear patterns better than Linear Regression
- Both models achieved high R2 scores due to the sequential nature of stock data
- Random Forest achieved lower MAE and RMSE, making it the better model

---

## Repository Structure

```
ArchTech-Internship/
├── Titanic_Survival_Classification.ipynb
├── Stock_Price_Prediction.ipynb
└── README.md
```

---

## How to Run

1. Open any notebook in Google Colab or Jupyter Notebook
2. Install required library for Task 2 if not already available:
   ```
   pip install yfinance
   ```
3. Run all cells from top to bottom
4. Titanic dataset loads automatically via `seaborn`
5. Stock data downloads automatically via `yfinance`

---

*Completed as part of the Arch Technologies Data Science Internship Program.*
