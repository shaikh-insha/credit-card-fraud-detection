# 💳 Credit Card Fraud Detection with ML & SMOTE

Detecting fraudulent transactions is essential in financial systems. This project uses various machine learning models, handles class imbalance with SMOTE, and evaluates models based on their fraud detection performance.

## 📌 Project Overview

This project aims to build and evaluate ML models for credit card fraud detection. It uses a synthetic dataset, performs data analysis, balances class distribution using SMOTE, and compares model performance using accuracy and F1-score.

---

## 📁 Dataset

The dataset `credit_card_data.csv` includes synthetic data with:

- `TransactionID`: Unique identifier  
- `TransactionAmount`: Amount in USD  
- `TransactionTime`: Time since the first transaction  
- `MerchantCategory`: Retail / Online / Restaurant / Travel  
- `CustomerAge`: Age (18–80)  
- `CustomerGender`: Male / Female  
- `CustomerIncome`: Income in USD (20,000–200,000)  
- `TransactionLocation`: Urban / Suburban / Rural  
- `PreviousFraudCount`: Count in past 6 months (0–5)  
- `Fraud`: Target variable (1 = fraud, 0 = not fraud)

---

## ⚙️ Features Used

- `TransactionAmount`, `TransactionTime`
- `MerchantCategory`, `CustomerAge`, `CustomerGender`
- `CustomerIncome`, `TransactionLocation`
- `PreviousFraudCount`

---

## 🔍 Exploratory Data Analysis (EDA)

- 📊 Correlation matrix
- 📦 Box plots (e.g., Fraud vs Amount)
- 📈 Fraud distribution bar chart
- 🧮 Count plots for categorical features

---

## 🧠 Machine Learning Models Used

| Model                | Accuracy   |
|---------------------|------------|
| Logistic Regression | 61.11%     |
| Random Forest       | 63.33%     |
| KNN                 | (Evaluated by F1-Score) |
| Decision Tree       | (Evaluated by F1-Score) |
| SVM (with SMOTE)    | (Evaluated by F1-Score) |

---

## 📈 F1-Score Comparison (Class 1: Fraud)

| Model                | F1-Score (Fraud Class) |
|---------------------|------------------------|
| Logistic Regression | 0.66                   |
| KNN                 | 0.75                   |
| Random Forest       | 0.78 ✅                |
| Decision Tree       | 0.72                   |
| SVM (with SMOTE)    | 0.71                   |

> ✅ **Random Forest** achieved the best fraud detection performance with an F1-score of 0.78.

---

## 📊 Visualizations

- Class distribution chart 
 <img width="765" height="573" alt="Screenshot 2025-07-13 at 8 08 02 pm" src="https://github.com/user-attachments/assets/99ad2e8f-6b20-4831-a5d1-fc429504fa20" />

- Accuracy bar graph
  <img width="922" height="542" alt="Screenshot 2025-07-13 at 8 18 01 pm" src="https://github.com/user-attachments/assets/35bbf85d-bb64-4432-9725-3296c32fcffd" />
  
- Confusion matrices (for each model in project)
  
- F1-score comparison chart
<img width="921" height="455" alt="Screenshot 2025-07-13 at 8 18 42 pm" src="https://github.com/user-attachments/assets/e7de1cff-b901-4455-bf1d-00f4f67ebbd3" />

---

## ✅ Conclusion

- Random Forest outperformed all other models, especially for the minority (fraud) class.
- SMOTE significantly improved the ability of models to detect fraud.
- Logistic Regression struggled with imbalanced data.
- F1-Score was a more reliable metric than accuracy in this problem.

---

## 🚀 Future Improvements

- Add advanced models like **XGBoost**, **LightGBM**, and **Ensemble Stacking**
- Hyperparameter tuning using **GridSearchCV**
- Introduce **external real-world datasets**
- Consider **deployment using Flask or Streamlit**

---

## 🧪 How to Run

```bash
# Clone the repo
git clone https://github.com/shaikh-insha/credit-card-fraud-detection.git
cd credit-card-fraud-detection

# Install dependencies
pip install -r requirements.txt

# Launch notebook
jupyter notebook CreditCardFraudDetection.ipynb
