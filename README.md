# 🏡 House Price Prediction using Machine Learning

This project solves the [Kaggle House Prices - Advanced Regression Techniques](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques) challenge. It predicts house prices using various regression techniques by focusing on data preprocessing, feature engineering, and model evaluation.

---

## 📁 Project Structure

# Main notebook with full ML pipeline
├── house_price.ipynb 

# Training dataset
├── train.csv 

# Test dataset
├── test.csv 

# Feature description file
├── data_description.txt

# This documentation
├── README.md



---

## 🎯 Objective

To predict the final sale price of homes in Ames, Iowa using 79 features describing each house. The goal is to minimize **Root Mean Squared Error (RMSE)** on the predictions.

---

## 🔍 Approach

1. 📥 Load and explore the dataset  
2. 🧹 Handle missing values properly (no `inplace=True` chained assignments)  
3. 🛠️ Feature engineering (`TotalSF`, `HouseAge`, etc.)  
4. 🔢 Convert categorical data using one-hot encoding  
5. ✂️ Split data into train & validation sets  
6. ⚖️ Scale features using `StandardScaler`  
7. 🤖 Train a Linear Regression model  
8. 📉 Evaluate with RMSE  
9. 📤 Predict test set and generate `submission.csv`  

---

## 🤖 Model

- `LinearRegression()` from `scikit-learn`  
- Evaluation metric: **RMSE**

You can easily extend it to:
- `RandomForestRegressor`
- `Ridge`, `Lasso`, or `XGBoost`

---

## 📦 Requirements

Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
