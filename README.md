# 🔒 Credit Card Fraud Detection Using Machine Learning

> ⚠️ **Work in Progress** - This project is currently under active development. Model training and evaluation phases are in progress.

## 📋 Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Project Objectives](#project-objectives)
- [Current Progress](#current-progress)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)

## 🎯 Overview

Credit card fraud represents a significant threat to the integrity of financial transactions and consumer trust in digital commerce. As the reliance on credit cards for everyday purchases continues to grow, so does the sophistication of fraudsters exploiting vulnerabilities in the system. 

This project aims to:
- Analyze patterns of credit card fraud
- Understand the factors contributing to fraudulent activities
- Develop machine learning models for fraud detection and prevention

## 📊 Dataset

**Source:** [Kaggle - Credit Card Fraud Dataset](https://www.kaggle.com/)

The dataset comprises **100,000 simulated transactions** designed to replicate real-world credit card activity.

### Features:
| Feature | Description |
|---------|-------------|
| `TransactionID` | Unique identifier for each transaction |
| `TransactionDate` | Date and time of the transaction |
| `Amount` | Monetary value of the transaction |
| `MerchantID` | Identifier for the merchant |
| `TransactionType` | Purchase or refund indicator |
| `Location` | Geographic location of the transaction |
| `IsFraud` | Binary target variable (1 = Fraud, 0 = Legitimate) |

## 🎯 Project Objectives

### 1. Exploratory Data Analysis (EDA)
- ✅ Examine distribution of transaction amounts and types
- ✅ Identify trends in transaction dates and locations
- ✅ Analyze the ratio of fraudulent to legitimate transactions
- ✅ Create comprehensive visualizations (12+ plots)

### 2. Pattern Recognition
- ✅ Analyze temporal patterns (hourly, daily, monthly fraud rates)
- ✅ Explore correlations between features and fraud occurrence
- ✅ Identify high-risk transaction characteristics

### 3. Fraud Detection Modeling
- 🔄 Implement Random Forest classifier
- ⏳ Evaluate model performance (accuracy, precision, recall, F1-score, ROC-AUC)
- ⏳ Perform hyperparameter tuning
- ⏳ Feature importance analysis


**Legend:** ✅ Completed | 🔄 In Progress | ⏳ Planned

## 📈 Current Progress

### ✅ Completed:
- Comprehensive EDA with 12 visualizations
- Temporal fraud pattern analysis (hour, day, month)
- Correlation matrix and feature analysis
- Fraud rate calculations across multiple time granularities
- Data preprocessing and feature engineering

### 🔄 In Progress:
- Random Forest model training
- Model evaluation and validation

### ⏳ Next Steps:
- Hyperparameter optimization
- Feature importance ranking

## 🛠️ Technologies Used

- **Python 3.13**
- **Data Analysis:** Pandas, NumPy
- **Visualization:** Matplotlib, Seaborn
- **Machine Learning:** Scikit-learn
- **Development Environment:** Jupyter Notebook
- **Version Control:** Git, GitHub

## 📥 Installation

### Prerequisites
- Python 3.8 or higher
- pip package manager

### Setup

1. **Clone the repository**
```bash
git clone https://github.com/yourusername/credit-card-fraud-detection.git
cd credit-card-fraud-detection
```

2. **Create a virtual environment**
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. **Install dependencies**
```bash
pip install -r requirements.txt
```

## 🚀 Usage

1. **Open Jupyter Notebook**
```bash
jupyter notebook
```

2. **Navigate to the notebook**
   - Open `fraud_detection_workflow.ipynb` to view the exploratory data analysis
   - Open `fraud_detection_model.ipynb` (coming soon) for model training

3. **Run the cells** sequentially to reproduce the analysis


