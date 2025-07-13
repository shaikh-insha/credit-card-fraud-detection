# 💳 Credit Card Fraud Detection

This project applies machine learning algorithms to detect fraudulent credit card transactions. It compares Logistic Regression and Random Forest using a synthetic dataset, implements SMOTE to address class imbalance, and visualizes results using confusion matrices and bar charts.

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

| **Model**             | **Accuracy** |
|-----------------------|--------------|
| Logistic Regression   | 61.11%       |
| Random Forest         | 63.33%       |

> Random Forest performed better, especially on imbalanced data.

## 📊 Visualizations
- Accuracy bar chart
  <img width="723" height="504" alt="Screenshot 2025-07-13 at 12 14 06 pm" src="https://github.com/user-attachments/assets/5463131e-9663-4f50-bcbe-1e82431d8620" />

- Confusion matrix plots
  x---
- Class-wise precision, recall, and F1-score
<img width="615" height="257" alt="Screenshot 2025-07-13 at 12 14 51 pm" src="https://github.com/user-attachments/assets/7dbcfe86-29c9-49ba-be9c-d1dac6fc4261" />
<img width="631" height="256" alt="Screenshot 2025-07-13 at 12 15 09 pm" src="https://github.com/user-attachments/assets/a4392b14-6187-4a19-a1d0-10b2fc4fc6d1" />


## 🚀 Improvements
- Use XGBoost or LightGBM
- Add more real-world features
- Tune hyperparameters & perform cross-validation

## 🧪 How to Run
Clone the repository  
```bash
git clone https://github.com/shaikh-insha/credit-card-fraud-detection.git
pip install -r requirements.txt
jupyter notebook CreditCardFraudDetection.ipynb
