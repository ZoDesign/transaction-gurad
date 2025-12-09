# 🔒 Credit Card Fraud Detection Using Machine Learning

> ⚠️ **Work in Progress** — This project is under active development. Model comparison, evaluation, and refinement phases are currently ongoing.

## 📋 Table of Contents

* [Overview](#overview)
* [Dataset](#dataset)
* [Data Quality Observations](#data-quality-observations)
* [Project Objectives](#project-objectives)
* [Current Progress](#current-progress)
* [Technologies Used](#technologies-used)
* [Installation](#installation)
* [Usage](#usage)

---

## 🎯 Overview

Credit card fraud poses a major threat to digital financial systems, with increasing transaction volumes creating opportunities for fraudulent activity. This project explores fraud detection using machine learning, focusing on understanding patterns in transaction behavior and evaluating multiple classification models.

What this project aims to achieve:

* Analyze transaction trends and fraud behaviour
* Evaluate the impact of data preprocessing and imbalanced class handling
* Compare multiple machine learning models to identify the best fraud detector
* Understand strengths and limitations of working with synthetic financial data

---

## 📊 Dataset

**Source:** *Kaggle — Credit Card Fraud Dataset (Simulated)*
**Transaction Count:** ~100,000 synthetic transactions

### Features:

| Feature           | Description                                 |
| ----------------- | ------------------------------------------- |
| `TransactionID`   | Unique identifier for each transaction      |
| `TransactionDate` | Timestamp of transaction                    |
| `Amount`          | Transaction amount                          |
| `MerchantID`      | Merchant identification code                |
| `TransactionType` | Purchase or refund                          |
| `Location`        | Geographic location                         |
| `IsFraud`         | Target variable (1 = Fraud, 0 = Legitimate) |

---

## ⚠️ Data Quality Observations

During analysis, several **limitations of the synthetic dataset** were identified:

* **Highly synthetic patterns** in several fields
* **Limited Feature Set** severely limiting model capability
* **Imbalanced classes** (fraud cases significantly lower than legitimate ones)
* **Weak correlations** between features and fraud, typical of simulated data


These considerations are now part of the project narrative to reflect real-world analytical thinking.

---

## 🎯 Project Objectives

### 1. Exploratory Data Analysis (EDA)

* ✅ Distribution analysis of transaction amounts & types
* ✅ Temporal trends (hourly, daily, monthly fraud rates)
* ✅ Fraud vs. legitimate class comparison
* ✅ 12+ visualizations (histograms, heatmaps)

### 2. Pattern Recognition

* ✅ Temporal fraud behaviour
* ✅ Feature correlation analysis
* ✅ Identification of high-risk transaction characteristics

### 3. Fraud Detection Modeling *(Updated Scope)*

Instead of training only one model, the project now compares **multiple classifiers**:

🔄 Planned Models:

* Logistic Regression
* Random Forest
* XGBoost
* Gradient Boosting

Evaluation Metrics:

* Precision
* Recall
* F1-score
* ROC-AUC
* Confusion matrix

**Legend:**
✅ Completed | 🔄 In Progress | ⏳ Planned

---

## 📈 Current Progress

### ✅ Completed:

* Full EDA with 12 visualizations
* Fraud pattern exploration (hour/day/month)
* Correlation matrix & statistical feature inspection
* Fraud rate calculation
* Data cleaning & preprocessing experimentation
* Identification of data quality issues and limitations

### 🔄 In Progress:

* Multi-model training pipeline
* Model evaluation and comparison

### ⏳ Next Steps:

* Identification of most suitable model 

---

## 🛠️ Technologies Used

* **Python 3.13**
* **Data Analysis:** Pandas, NumPy
* **Visualization:** Matplotlib, Seaborn
* **Machine Learning:** Scikit-learn, XGBoost
* **Dev Environment:** Jupyter Notebook
* **Version Control:** Git & GitHub

---

## 📥 Installation

### Prerequisites

* Python 3.8+
* pip

### Setup

```bash
git clone https://github.com/yourusername/credit-card-fraud-detection.git
cd credit-card-fraud-detection
```

Create a virtual environment:

```bash
python -m venv venv
source venv/bin/activate       # Windows: venv\Scripts\activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## 🚀 Usage

Open Jupyter Notebook:

```bash
jupyter notebook
```

### Notebooks:

* `fraud_detection_workflow.ipynb` — EDA & preprocessing
* `model_comparison.ipynb` — Multiple classifiers (in progress)

Run cells sequentially to reproduce the analysis.
