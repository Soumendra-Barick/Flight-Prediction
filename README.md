<h1 align="center">✈️ Flight Price Prediction</h1>

<p align="center">
  Predicting airline ticket prices using Machine Learning.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.8-blue" />
  <img src="https://img.shields.io/badge/ML-RandomForest-green" />
  <img src="https://img.shields.io/badge/License-MIT-lightgrey" />
</p>

---

## 📌 Overview

This project uses machine learning techniques to predict flight ticket prices based on various parameters such as airline, source, destination, travel dates, and more. It includes complete data preprocessing, feature engineering, model training, and evaluation.

---

## 🧠 Tech Stack

- **Language**: Python 🐍  
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn  
- **Model**: Random Forest Regressor  
- **IDE**: Jupyter Notebook

---

## 📂 Dataset

- `Train_data.csv`: Includes the target variable `Price`
- `Test_data.csv`: Used for final prediction (without price column)

---

## 🔧 Feature Engineering

- Extracted day/month from journey date  
- Parsed hours and minutes from `Dep_Time`, `Arrival_Time`, and `Duration`  
- Encoded categorical variables using One-Hot Encoding  
- Removed outliers and missing values

---

## 📁 Project Structure

flight-price-prediction/
│
├── data/
│   ├── Train_data.csv
│   └── Test_data.csv
│
├── Flight_Price_Prediction.ipynb
├── README.md
└── LICENSE

---

## 🚀 Model Training

```python
from sklearn.ensemble import RandomForestRegressor
from sklearn.model_selection import train_test_split
from sklearn.metrics import mean_squared_error
