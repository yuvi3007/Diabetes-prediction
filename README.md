# Diabetes Risk Prediction 🩺🔍

A machine learning project aimed at predicting diabetes presence in patients using a real-world medical dataset. The dataset contained **100,000+ records** and presented real-world complexities like **missing values** and **severe class imbalance** — making it a perfect case study for advanced model handling.

## 📌 Objective

To build a robust classification model that can accurately identify high-risk diabetic patients despite data quality issues and class imbalance, thus aiding early diagnosis and preventive care.

---

## 📊 Dataset Overview

- **Rows**: ~100,000+
- **Target**: Binary label indicating diabetes (1 = positive, 0 = negative)
- **Challenges**:
  - Missing values across several features
  - **Highly imbalanced classes** (significantly fewer positives)
  - Presence of noisy entries and outliers

---

## 🛠️ Workflow Summary

### ✅ Data Preprocessing
- Imputation of missing values using **mean/median strategy**
- Outlier treatment using **IQR method**
- Feature scaling using **StandardScaler**

### ✅ Handling Class Imbalance
- Applied **SMOTE (Synthetic Minority Over-sampling Technique)**
- Balanced class distribution prior to model training
- Improved recall without sacrificing precision

### ✅ Model Training
- Trained **Random Forest Classifier** with hyperparameter tuning via **GridSearchCV**
- Used stratified splitting to maintain class ratio in train/test sets
- Evaluated using **F1 Score**, **Precision**, **Recall**, and **Confusion Matrix**

---

## 🚀 Technologies Used

- **Language**: Python
- **Libraries**:
  - pandas, numpy
  - scikit-learn
  - imbalanced-learn (for SMOTE)
  - matplotlib, seaborn (for EDA and plots)

---

## 🧪 Model Performance

| Metric      | Before SMOTE | After SMOTE |
|-------------|--------------|-------------|
| Accuracy    | 0.88         | 0.96        |
| Precision   | 0.85         | 0.96        |
| Recall      | 0.70         | 0.99        |
| **F1 Score**| **0.79**     | **0.98**    |

> 🎯 SMOTE drastically improved the model's ability to detect diabetic patients, making it more usable in real clinical settings.

---


