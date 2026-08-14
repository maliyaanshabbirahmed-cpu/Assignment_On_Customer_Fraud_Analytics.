# Assignment_On_Customer_Fraud_Analytics.
A comprehensive machine learning assignment analyzing customer data to detect fraudulent transactions, handling data preprocessing, class imbalance, and model evaluation.
# Assignment: Customer Fraud Analytics & Detection

## 📌 Project Overview
This repository contains the code, analysis, and models for the **Customer Fraud Analytics** assignment. The goal is to build, evaluate, and fine-tune machine learning classification models to accurately detect fraudulent customer behavior using behavioral and demographic metrics.

---

## 📊 Dataset Specifications (`customer_analytics_dataset.csv`)
* **Total Records:** 5,000 customers[cite: 1]
* **Features:** 13 attributes including demographic details, transaction history, and engagement metrics[cite: 1]
* **Target Variable:** `is_fraudulent` (Binary: `0` = Legitimate, `1` = Fraudulent)[cite: 1]

### Key Data Insights:
* **Missing Values:** Found in `avg_order_value` (250 missing) and `email_open_rate` (250 missing)[cite: 1].
* **Class Imbalance:** Highly imbalanced distribution (~97.42% legitimate vs. ~2.58% fraudulent)[cite: 1].

---

## 🛠️ Key Steps & Methodology

1. **Exploratory Data Analysis (EDA):**
   * Audited data types, distributions, and summary statistics.
   * Visualized class distribution and feature correlations.

2. **Data Preprocessing & Cleaning:**
   * Handled missing values via proper imputation techniques.
   * Dropped non-predictive identifiers like `customer_id`[cite: 1].
   * Processed date-time fields (`customer_since`)[cite: 1] and encoded categorical columns.

3. **Handling Class Imbalance:**
   * Applied **SMOTE** (Synthetic Minority Over-sampling Technique) on the training dataset to resolve the 97:3 class ratio discrepancy[cite: 1].

4. **Model Training & Evaluation:**
   * Built baseline models (Decision Trees, Random Forest, and XGBoost).
   * Evaluated model performance utilizing appropriate metrics like Precision, Recall, F1-Score, and ROC-AUC (given the severe class imbalance).

---

## 🚀 Getting Started

1. Clone the repository:
   ```bash
   git clone [https://github.com/maliyaanshabbirahmed-cpu/Assignment_On_Customer_Fraud_Analytics.git](https://github.com/maliyaanshabbirahmed-cpu/Assignment_On_Customer_Fraud_Analytics.git)
