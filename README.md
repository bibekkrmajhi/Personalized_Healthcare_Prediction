# 🏥 Personalized Healthcare Prediction System


### Diabetes Risk Prediction using Machine Learning

### 📌 Project Overview

The Personalized Healthcare Prediction System is a machine learning–based project that predicts an individual’s Diabetes Risk (Low, Medium, High) using a comprehensive patient health dataset.

The system analyzes demographic, clinical, lifestyle, and family-history features to generate personalized risk predictions, supporting early detection and preventive healthcare decision-making.

### 🎯 Problem Statement

Diabetes is a chronic disease that often goes undiagnosed until complications arise. Early detection of risk can significantly improve prevention and treatment outcomes.

**The objective of this project is to:**

- Analyze patient healthcare data

- Build a predictive model for diabetes risk

- Generate personalized risk insights

- Evaluate model performance using classification metrics

### 🧠 Solution Approach

This project uses a supervised machine learning classification approach to:

- Learn patterns from historical healthcare data

- Predict diabetes risk for unseen patient profiles

- Support personalized healthcare recommendations

Unlike rule-based systems, the model evaluates multiple health factors together, closely reflecting real-world medical decision-making.

### 📂 Dataset Description

The dataset contains approximately **40 healthcare-related features**, including:

**👤 Demographic Features**

- Age

- Gender

**🏥 Clinical Features**

- Glucose Level

- HbA1c

- BMI

- Blood Pressure

- Cholesterol

### 🏃 Lifestyle Features

- Physical Activity Level

- Alcohol Consumption

- Sleep

- Stress

### 🧬 Family & Genetic Indicators

- Family History

- Genetic Risk Factors

### 🎯 Target Variable

- Diabetes_Risk

     - Low

     - Moderate

     - High

⚠️ Columns that could cause data leakage (recommendations, outcome-based fields) were excluded from model training.

### 🛠️ Technologies Used
**Programming & Tools**

- Python

- Jupyter Notebook

- Libraries

- pandas

- numpy

- scikit-learn

- matplotlib

- seaborn

### ⚙️ Project Workflow
#### 1️⃣ Data Loading & Exploration

Loaded dataset and examined structure

Identified missing values and data types

#### 2️⃣ Data Preprocessing

Handled missing values

Encoded categorical variables

Standardized numerical features

Ensured data leakage prevention

#### 3️⃣ Feature Selection

Selected relevant health features

Removed target-related and derived columns

#### 4️⃣ Model Building

Implemented Random Forest Classifier

Used Scikit-learn Pipeline for clean preprocessing and training

#### 5️⃣ Model Evaluation

Evaluated model performance on test data

Verified consistency of predictions

#### 6️⃣ Testing with New Patient Data (Step 15)

Tested the trained model with unseen patient profiles

Ensured schema and datatype consistency

Successfully generated diabetes risk predictions

#### 7️⃣ Personalized Recommendation

Mapped predicted risk levels to healthcare recommendations

### 📊 Model Performance

The Random Forest model demonstrated reliable predictive performance on the test dataset and showed stable generalization on unseen patient data and achieved 81.25% accuracy.

✅ **Accuracy: 81.25%**

📋**Classification Report Summary**

| Risk Level | Precision | Recall | F1-Score |
| ---------- | --------- | ------ | -------- |
| High       | 1.00      | 0.11   | 0.20     |
| Low        | 0.83      | 1.00   | 0.91     |
| Moderate   | 0.60      | 0.26   | 0.37     |


### 🔎 Key Observations

- Model performs very well for Low-risk patients

- High-risk predictions are precise but have lower recall

- Moderate-risk category is affected by class imbalance



### New Patient Prediction Example

new_patient = X.iloc[[0]].copy()

new_patient["Age"] = 55

new_patient["Glucose_Level"] = 185

new_patient["HbA1c"] = 8.3

new_patient["Family_History_T2D"] = 1

new_patient["APOE_e4_Carrier"] = 1


### 💡 Personalized Recommendation Logic

**Low Risk** → Maintain a healthy diet and regular physical activity

**Moderate Risk** → ifestyle modifications advised. Monitor blood glucose regularly

**High Risk** → Consult a physician immediately. Strict diet, exercise, and medical supervision required


**Sample Output:**

Predicted Diabetes Risk: **Low**

### 🧠 Key Insight

A high glucose level alone does not guarantee a high diabetes risk.
The model evaluates all health features together, making it a multivariate and personalized prediction system.

### 📈 Results & Impact

- Successfully predicts diabetes risk categories

- Demonstrates practical application of ML in healthcare

- Highlights importance of personalized, data-driven health assessment


### ✅ Conclusion

Built a complete end-to-end Personalized Healthcare Prediction System

Applied industry-standard machine learning practices

Validated predictions using unseen patient data



### 🚀 Future Enhancements

- Deploy as a web application (Flask / Streamlit)

- Add model explainability (feature importance / SHAP)

- Integrate real-time patient data input

- Extend system to predict additional health risks


### 👤 Author

**Bibek Kumar Majhi**

Data Analytics & Machine Learning Enthusiast

