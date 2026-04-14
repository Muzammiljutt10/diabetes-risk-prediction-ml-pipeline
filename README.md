# diabetes-risk-prediction-ml-pipeline
XGBoost-based classification model for diabetes prediction with feature engineering, class imbalance handling (scale_pos_weight), and decision threshold tuning for improved precision-recall balance.

# Diabetes Risk Prediction using XGBoost


##  Overview

This project focuses on predicting diabetes risk using a machine learning classification model built with **XGBoost**.  
It addresses **class imbalance** and improves model performance using **threshold tuning** to achieve a better balance between precision and recall.

---

##  Objectives

- Predict whether a patient is diabetic or non-diabetic
- Handle **imbalanced dataset** effectively
- Optimize model performance beyond accuracy
- Improve **precision-recall trade-off** using threshold tuning

---

## 📊 Dataset Features

The model is trained on the following features:

- `gender`
- `age`
- `hypertension`
- `heart_disease`
- `smoking_history`
- `bmi`
- `HbA1c_level`
- `blood_glucose_level`

---

## ⚙️ Data Preprocessing

- Categorical encoding:
  - `gender`, `smoking_history`
- Feature scaling:
  - `age`, `bmi`, `HbA1c_level`, `blood_glucose_level`
- Train-test split applied
- Class imbalance handled using:
  - `scale_pos_weight` in XGBoost

---

## 🤖 Model Used

- **XGBoost Classifier**

### Key Parameters:
```python
max_depth=4
n_estimators=300
learning_rate=0.08
subsample=0.8
colsample_bytree=0.8
scale_pos_weight=imbalanced_ratio
reg_alpha=0.5
reg_lambda=1
