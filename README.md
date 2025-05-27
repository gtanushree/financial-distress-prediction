# 💼 Financial Distress Prediction

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![Build Status](https://img.shields.io/badge/Status-Active-brightgreen.svg)]()
[![F1 Score](https://img.shields.io/badge/Evaluation-F1--Score-important)]()

Predicting financial distress in companies using multivariate time-series data with financial and non-financial features. This project explores various machine learning and deep learning models including classification, regression, and LSTM-based time-series classification.

---

## 📁 Dataset Overview

The dataset contains time-series data from multiple companies with financial metrics across different time periods.

- **Company**: Company identifier
- **Time**: Time period (1–14)
- **Financial Distress** *(Target)*:
  - `1`: Financially distressed (value ≤ -0.50)
  - `0`: Healthy
- **x1 to x83**: Financial and non-financial features  
  - `x80`: Categorical variable

⚠️ **Imbalanced Dataset**:
- 136 firm-years → Financially Distressed  
- 3546 firm-years → Healthy  
- Performance metric: **F1-Score**

---

## 🔍 Project Objectives

- Build a predictive model for financial distress classification.
- Compare classification, regression-to-classification, and time-series approaches.
- Handle class imbalance effectively.
- Evaluate using precision, recall, and F1-score.

---

## 📊 Modeling Approaches

| Approach                        | Tools / Models                   |
|-------------------------------|----------------------------------|
| Classification                | Logistic Regression, XGBoost     |
| Regression-to-Classification | Linear Regression, SVR           |
| Time-Series Classification    | LSTM, GRU, Temporal CNN          |

---

## 🏗️ Project Structure

financial-distress-prediction/
├── data/
│ └── Financial Distress.csv # Raw dataset
├── notebooks/
│ ├── 01_EDA.ipynb # Exploratory analysis
│ ├── 02_Classification.ipynb # ML classification models
│ ├── 03_Regression.ipynb # Regression-based modeling
│ └── 04_LSTM_TimeSeries.ipynb # LSTM-based model
├── models/
│ └── best_model.pkl # Saved best-performing model
├── requirements.txt # Python dependencies
└── README.md # Project documentation

---

## 🚀 Getting Started

### 🔧 Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/gtanushree/financial-distress-prediction.git
   cd financial-distress-prediction

2. Install required packages:
    ```bash
    pip install -r requirements.txt

### ▶️ Running the Project
Launch a Jupyter Notebook and explore the project:
    ```bash
    jupyter notebook

## ✅ Evaluation Metrics
F1 Score (primary)

Precision

Recall

Confusion Matrix

ROC-AUC (optional)

## 📌 Notes
Ensure that the time-dependent nature of the data is respected (no future data leakage).

Consider balancing techniques such as SMOTE or class weighting.

Feature x80 requires encoding (OneHot or LabelEncoding).

## 📬 Contact
For questions or collaboration:

📧 gtanushree534@gmail.com

🌐 www.linkedin.com/in/tanu-shree-gupta-7445a927b

## 📝 License
This project is licensed under the MIT License.
   

