# Heart Attack Risk Prediction Using Machine Learning

## 🚀 Overview

This project focuses on predicting **heart attack risk** using machine learning techniques, leveraging a processed health dataset with a strong emphasis on early diagnosis. The model achieves an **accuracy of 85%**, making it a robust prototype for healthcare analytics and clinical testing environments.

This work is inspired by approaches used in youth diabetes risk modeling but is reoriented towards **cardiovascular risk prediction**, particularly **heart attacks**. The project is research-driven and aims to serve as a scalable baseline for healthcare tech innovation.

## 📊 Table of Contents

1. [Problem Statement](#problem-statement)
2. [Dataset](#dataset)
3. [Data Preprocessing](#data-preprocessing)
4. [Modeling & Evaluation](#modeling--evaluation)
5. [Results](#results)
6. [Future Scope](#future-scope)
7. [References](#references)

## ⚠️ Problem Statement

Heart disease is the leading cause of death globally. Many fatal heart attacks occur without any prior symptoms, underscoring the need for **predictive tools that can assess cardiovascular risk in advance**. This project aims to use machine learning to:

* Predict the likelihood of a person having a heart attack
* Enable early medical intervention and lifestyle correction
* Improve diagnostic accuracy through data-driven insights

## 📁 Dataset

* The dataset contains **clinical features** like age, cholesterol, blood pressure, fasting blood sugar, and more.
* Source: Publicly available datasets similar to those from [UCI Heart Disease Repository](https://archive.ics.uci.edu/ml/datasets/heart+disease) (adapted for this project).

### Features Included

* Age
* Sex
* Chest Pain Type
* Resting Blood Pressure
* Serum Cholesterol
* Fasting Blood Sugar
* Rest ECG Results
* Maximum Heart Rate
* Exercise-Induced Angina
* ST Depression
* Slope of ST Segment
* Number of Major Vessels
* Thalassemia

## 🧹 Data Preprocessing

* **Missing Values**: Handled with imputation strategies
* **Normalization**: Applied MinMaxScaler
* **Encoding**: Categorical features label-encoded
* **Oversampling**: Used SMOTE to address class imbalance

## 🧠 Modeling & Evaluation

### ML Algorithms Used

* **Logistic Regression**
* **Random Forest**
* **Naive Bayes**
* **Decision Tree**

### Evaluation Metrics

* **Accuracy**
* **Recall (Sensitivity)**
* **Precision**
* **Specificity**
* **F1 Score**

> ✅ **Best performing model**: Logistic Regression with **85% accuracy** and balanced performance across other metrics.

## 📈 Results Summary

| Model                   | Accuracy | Precision | Recall   | Specificity | F1 Score |
| ----------------------- | -------- | --------- | -------- | ----------- | -------- |
| **Logistic Regression** | 85%      | High      | High     | High        | High     |
| Random Forest           | 81%      | Moderate  | Moderate | High        | Moderate |
| Naive Bayes             | 74%      | Low       | High     | Moderate    | Low      |
| Decision Tree           | 78%      | Moderate  | Moderate | Moderate    | Moderate |

## 🔭 Future Scope

* **Deep Learning Models**: Integrate CNN/RNNs for temporal and ECG-based features.
* **Mobile App Integration**: Real-time prediction using health APIs (e.g., Apple HealthKit, Google Fit).
* **Explainability**: Use SHAP/LIME to interpret predictions.
* **Clinical Trials**: Collaborate with hospitals to validate model in real-world settings.

## 📚 References

* Original framework adapted from: "[Predicting youth diabetes risk using NHANES data and machine learning](https://doi.org/10.1038/s41598-021-90406-0)"
* [UCI Heart Disease Dataset](https://archive.ics.uci.edu/ml/datasets/heart+disease)
