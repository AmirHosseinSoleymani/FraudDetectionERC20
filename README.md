# 🔍 Fraud Detection on ERC20 Transactions

## 📌 Overview
This repository contains an implementation of fraud detection on **ERC20 token transactions** using machine learning models such as **CatBoost, Logistic Regression, Random Forest, and XGBoost**. The goal is to classify transactions as fraudulent or legitimate based on historical transaction data.

## 📂 Dataset
The dataset includes **Ethereum-based ERC20 transactions** with features such as:
- 'FLAG', 'Avg min between sent tnx', 'Avg min between received tnx',
       'Time Diff between first and last (Mins)', 'Sent tnx', 'Received Tnx',
       'Number of Created Contracts', 'max value received ',
       'avg val received', 'avg val sent', 'min value sent to contract',
       'total Ether sent', 'total ether balance',
       ' ERC20 total Ether received', ' ERC20 total ether sent',
       ' ERC20 total Ether sent contract', ' ERC20 uniq sent addr',
       ' ERC20 uniq sent addr.1', ' ERC20 uniq rec token name'

## 📖 Models Used
The project implements multiple **classification algorithms**:
- **CatBoost** 🟡 (Gradient boosting for categorical data)
- **Logistic Regression** 🔵 (Linear classification model)
- **Random Forest** 🌳 (Ensemble of decision trees)
- **XGBoost** 🔥 (Optimized gradient boosting)

Each model is trained and evaluated using appropriate metrics such as **Accuracy, Precision, Recall, F1-score, and AUC-ROC.**


## 📊 Performance & Results
The Best Model (CatBoost):
| Class | Precision | Recall | F1-Score | Support |
|-------|-----------|--------|----------|---------|
| 0     | 0.99      | 0.98   | 0.99     | 1547    |
| 1    | 0.93      | 0.96   | 0.95     | 422     |

**Accuracy**: 0.98 (1969 samples)  
**Macro avg**: Precision: 0.96, Recall: 0.97, F1-score: 0.97  
**Weighted avg**: Precision: 0.98, Recall: 0.98, F1-score: 0.98

**Confusion Matrix
|          | Predicted 0 | Predicted -1 |
|----------|-------------|--------------|
| True 0   | 1518        | 29           |
| True 1  | 16          | 406          |


## 📌 Future Improvements
- Feature engineering for **better fraud pattern detection**
- Implement **deep learning models** (e.g., LSTMs for transaction sequences)
- Deploy as an **API or real-time fraud detection system**

## 🤝 Contributing
Contributions are welcome! Feel free to open an issue or submit a pull request.

## 📜 License
This project is licensed under the **MIT License**.

---
💡 **Developed by [AmirHosseinSoleymani]** | 🚀 Follow for more AI & Blockchain projects!
