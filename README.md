#  Diabetes Risk Prediction using Machine Learning

##  Project Overview
This project focuses on predicting the likelihood of diabetes using machine learning techniques on a **large-scale dataset (100,000 records)**. The model leverages health-related features to classify individuals as diabetic or non-diabetic.

The objective is to build a reliable prediction system that can assist in early detection and healthcare decision-making.

---

##  Dataset
- The dataset contains **~100,000 samples**, making it suitable for training robust machine learning models.
- Features include:
  - Age  
  - Gender  
  - BMI (Body Mass Index)  
  - Hypertension  
  - Heart Disease  
  - Smoking History  
  - HbA1c Level  
  - Blood Glucose Level  

- Target Variable:
  - `0` → Non-diabetic  
  - `1` → Diabetic  

---

## Project Workflow

###  Importing Libraries
Core libraries used:
- NumPy  
- Pandas  
- Matplotlib / Seaborn  
- Scikit-learn  
- XGBoost  

---

###  Data Loading & Exploration
- Dataset loaded using Pandas  
- Initial exploration:
  - `.head()`  
  - `.info()`  
  - `.describe()`  

---

###  Data Preprocessing
- Encoding categorical variables (Gender, Smoking history)  
- Handling missing values  
- Preparing features for model input  

---

###  Exploratory Data Analysis (EDA)
- Distribution plots (`sns.displot`)  
- Correlation heatmap  
- Feature relationships with target  

---

###  Feature Scaling
- Applied StandardScaler to numerical features  

---

###  Train-Test Split
- Split dataset into training and testing sets  

---

###  Model Training
- Model: **XGBoost Classifier**  

---

### Model Evaluation
- Training Accuracy: ~82.8%  
- Testing Accuracy: ~80.5%  
- Cross-validation score: ~77.3%    

---

###  Prediction System
- Takes user input  
- Applies preprocessing & scaling  
- Outputs prediction  

---


##  Technologies Used
- Python  
- Pandas, NumPy  
- Scikit-learn  
- XGBoost  
- Matplotlib, Seaborn  

---

##  Conclusion
This project demonstrates the application of machine learning on a **large dataset (100k records)** to predict diabetes risk, with scope for further improvement in recall and real-world deployment.
