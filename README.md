# 🏦 Binary Classification with Bank Dataset (Kaggle)

This project is a solution to the Kaggle competition:

**Binary Classification with a Bank Dataset – Clone**

The goal is to predict the probability of a client subscribing to a term deposit using tabular customer data.

---

## 🎯 Objective

- Perform binary classification
- Optimize model using **ROC-AUC**
- Implement proper cross-validation
- Prevent data leakage
- Generate Kaggle-ready submission file

---

## 📊 Dataset Overview

The dataset contains customer information such as:

- Age
- Job
- Marital status
- Education
- Default
- Balance
- Housing loan
- Contact type
- Campaign details
- Previous outcome
- Target variable: `y`

Target variable:
- `1` → Subscribed
- `0` → Not Subscribed

---

## 🧠 Approach

### 1️⃣ Data Preprocessing
- Removed missing target values
- Converted categorical variables using Label Encoding
- Ensured train/test feature alignment

### 2️⃣ Validation Strategy
- 5-Fold Stratified KFold
- Shuffle enabled
- Fixed random seed for reproducibility

### 3️⃣ Model Used
- **LightGBM Classifier**
- Early stopping (100 rounds)
- Learning rate = 0.05
- 1000 estimators

### 4️⃣ Evaluation Metric
- ROC-AUC (Primary competition metric)

---

## 📈 Model Performance

| Metric | Score |
|--------|-------|
| Cross-Validation AUC | **0.96915** |
| Validation Strategy | 5-Fold Stratified |
| Model | LightGBM |

---

## 📁 Project Structure
📦 Bank-Binary-Classification
┣ 📄 train.csv
┣ 📄 test.csv
┣ 📄 submission.csv
┣ 📓 bank_classification.ipynb
┗ 📄 README.md

## 🔗 Google Colab Notebook

You can view and run the complete implementation using Google Colab at the link below:

👉 https://colab.research.google.com/drive/1PDECBqg8cf7ZfZ8cWhqcyKAuY3AJLnxZ?usp=sharing

