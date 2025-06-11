# 💳 Credit Card Fraud Detection

This project detects fraudulent credit card transactions using machine learning. It includes a trained XGBoost model, SHAP explainability, and a live prediction web app built with Streamlit.

---

## 🚀 Project Overview

Fraud detection is critical for financial institutions and businesses. This project analyzes anonymized credit card transaction data to identify fraudulent behavior using supervised learning and explainable AI.

---

## 🧠 Objectives

- Detect fraudulent transactions in a highly imbalanced dataset
- Use XGBoost classifier for high accuracy and robustness
- Apply SMOTE to balance class distribution
- Visualize model performance and interpret predictions using SHAP
- Build an interactive prediction tool using Streamlit

---

## 🗃️ Dataset

- Source: [Kaggle Credit Card Fraud Detection Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- Transactions made by European cardholders in September 2013
- 284,807 transactions with 492 frauds (0.172%)

---

## 📊 Features Used

- `Time`: Seconds elapsed between the transaction and the first transaction
- `V1` to `V28`: PCA-anonymized features
- `Amount`: Transaction amount
- `Class`: Target variable (`0` = Legitimate, `1` = Fraudulent)

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| **Python** | Core language |
| **Pandas, NumPy** | Data manipulation |
| **Matplotlib, Seaborn** | Visualization |
| **XGBoost** | Classifier |
| **SMOTE** | Handling imbalanced data |
| **SHAP** | Model explainability |
| **Streamlit** | Web app for predictions |
| **Joblib** | Model serialization |

---

## 🔍 Model Training Highlights

1. **Data Preprocessing**
   - Scaled `Time` and `Amount` features using `StandardScaler`
   - Addressed class imbalance with SMOTE

2. **Model**
   - Trained `XGBoostClassifier` with balanced data
   - Evaluated with precision, recall, F1-score, and ROC-AUC

3. **Explainability**
   - Used SHAP to understand feature importance and individual predictions

---

## 📈 Performance

| Metric | Score |
|--------|-------|
| Accuracy | ~99.9% |
| Recall (Fraud) | High |
| ROC-AUC | Excellent |

> Note: Due to data imbalance, recall and precision are more important than accuracy.

---

## 🌐 Web App Preview

A simple app for entering transaction data and predicting if it is **fraudulent** or **legitimate**.

### ▶️ How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/credit-card-fraud-detection.git
   cd credit-card-fraud-detection
