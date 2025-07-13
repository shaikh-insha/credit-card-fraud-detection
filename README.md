# 💳 Credit Card Fraud Detection

A machine learning project to classify fraudulent credit card transactions using Logistic Regression and Random Forest. Includes SMOTE for class balancing, EDA, and detailed evaluation.

## 📁 Dataset
A small sample dataset (`credit_card_data.csv`) with:
- Transaction details
- Customer info (age, gender, income, etc.)
- Fraud label (1 = fraud, 0 = not fraud)

## ⚙️ Features Used
- Transaction Amount, Time, Merchant Category
- Customer Age, Gender, Income
- Transaction Location
- Past Fraud Count

## 🔍 Exploratory Data Analysis (EDA)
- Correlation matrix
- Distribution plots
- Box plots for fraud vs amount

## 🔁 Models Compared
| Model              | Accuracy |
|-------------------|----------|
| Logistic Regression | 61.11%   |
| Random Forest       | 63.33%   |

> Random Forest performed better, especially on imbalanced data.

## 📊 Visualizations
- Accuracy bar chart
- Confusion matrix plots
- Class-wise precision, recall, and F1-score

## 🚀 Improvements
- Use XGBoost or LightGBM
- Add more real-world features
- Tune hyperparameters & perform cross-validation

## 🧪 How to Run
```bash
pip install -r requirements.txt
jupyter notebook CreditCardFraudDetection.ipynb
