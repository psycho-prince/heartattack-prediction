# Predicting Youth Diabetes Mellitus (DM) Risk

## Overview

This project is an **iteration of the paper titled "[Predicting youth diabetes risk using NHANES data and machine learning](https://doi.org/10.1038/s41598-021-90406-0),"** which was published in the *Scientific Reports* journal. The original study set a precedent in using machine learning to predict diabetes risk among youth, and this project aims to build on that foundation by enhancing the predictive models and expanding the dataset.

**Purpose of the Original Paper**:
Prediabetes and diabetes mellitus (preDM/DM) have become alarmingly prevalent among youth in recent years. However, simple questionnaire-based screening tools to reliably assess diabetes risk are only available for adults, not youth. As a first step in developing such a tool, the original paper used a large-scale dataset from the National Health and Nutritional Examination Survey (NHANES) to examine the performance of a published pediatric clinical screening guideline in identifying youth with preDM/DM based on American Diabetes Association diagnostic biomarkers.

The study assessed the agreement between the clinical guideline and biomarker criteria using established evaluation measures (sensitivity, specificity, positive/negative predictive value, F-measure for the positive/negative preDM/DM classes, and Kappa). It also compared the performance of the guideline to those of machine learning (ML)-based preDM/DM classifiers derived from the NHANES dataset. The results indicated that the clinical guideline did not perform well in identifying preDM/DM status among youth, highlighting the need for further development of a simple yet accurate screener for youth diabetes risk, potentially using advanced ML methods and a broader range of clinical and behavioral health data.

**Note**: The final dataset used in the original paper was not available, so for this project, the data was gathered directly from the NHANES website to reiterate the study.

## Table of Contents

1. [Problem Definition](#problem-definition)
2. [Dataset](#dataset)
3. [Data Management and Preprocessing](#data-management-and-preprocessing)
4. [Modeling and Evaluation](#modeling-and-evaluation)
5. [Results](#results)
6. [Future Work and Recommendations](#future-work-and-recommendations)
7. [References](#references)

## Problem Definition

Diabetes Mellitus is a growing concern among youth, with increasing cases of prediabetes and diabetes being reported. Early diagnosis is often challenging due to the insufficient screening tools currently available. This project focuses on improving the accuracy and reliability of early diabetes prediction by leveraging advanced machine learning models.

## Dataset

The dataset used in this project includes various health and demographic factors related to youth aged 12-19. The data was collected from multiple sources, and significant preprocessing steps were performed to ensure the quality and relevance of the dataset.

### Data Collection and Cleaning

- **Sources**: The data was compiled from medical records, laboratory tests, and health surveys.
- **Cleaning**: The dataset underwent rigorous cleaning processes, including handling missing values, correcting data types, and normalizing the data.

### Exploratory Data Analysis (EDA)

An exploratory analysis was conducted to understand the distribution of key variables and identify potential relationships between different features. This step was crucial in guiding the selection of relevant features for the predictive models.

## Data Management and Preprocessing

Data management and preprocessing steps were implemented to prepare the dataset for modeling. The primary steps include:

1. **Data Transformation**: Numerical and categorical features were transformed using appropriate techniques.
2. **Feature Engineering**: New features were created to enhance the model's predictive power.
3. **Oversampling**: Given the class imbalance in the dataset, oversampling techniques were applied to ensure the models could accurately predict both positive and negative cases.

## Modeling and Evaluation

Multiple machine learning models were implemented and evaluated to identify the best approach for predicting diabetes risk.

### Models Used

1. **Logistic Regression**
2. **Decision Tree**
3. **Random Forest**
4. **Naive Bayes**

### Evaluation Metrics

Each model was evaluated using the following metrics:

- **Accuracy**: The percentage of correct predictions made by the model.
- **Sensitivity (Recall)**: The ability of the model to correctly identify positive cases.
- **Specificity**: The ability of the model to correctly identify negative cases.
- **Precision (PPV)**: The proportion of true positive predictions out of all positive predictions.
- **Negative Predictive Value (NPV)**: The proportion of true negative predictions out of all negative predictions.
- **F1 Score**: The harmonic mean of precision and recall, providing a balance between the two metrics.

## Results

The models demonstrated varying levels of performance across different metrics. Key findings include:

- **Naive Bayes**: Showed high specificity but low sensitivity, making it suitable for reducing false positives.
- **Logistic Regression**: Balanced performance across sensitivity, specificity, and accuracy, making it a strong candidate for a comprehensive prediction approach.
- **Decision Tree and Random Forest**: Provided insights into the importance of different features but exhibited varying performance depending on the metric considered.

### Summary of Results

| Model               | Accuracy | Sensitivity | Specificity | PPV  | NPV  | F1 Score |
|---------------------|----------|-------------|-------------|------|------|----------|
| **Naive Bayes**     | 67.6%    | 18.5%       | 87.7%       | 38.2%| 72.4%| 24.9%    |
| **Random Forest**   | 62.6%    | 39.5%       | 72.1%       | 36.7%| 74.4%| 38.0%    |
| **Decision Tree**   | 69.2%    | 32.5%       | 84.2%       | 45.7%| 75.3%| 36.0%    |
| **Logistic Regression** | 58.5% | 45.9%       | 63.7%       | 34.1%| 74.1%| 39.1%    |

## Future Work and Recommendations

Based on the current findings, the following recommendations and areas for future work are proposed:

1. **Data Update**: Integrating more recent data (up to 2022) to enhance the model's accuracy and reliability.
2. **Long-term Disease Data**: Including data on long-term complications such as diabetic coma to improve the model’s predictive power over extended periods.
3. **Metabolic Conditions**: Investigating the impact of metabolic conditions like high cholesterol and hormonal imbalances on diabetes risk.
4. **Growth Indicators**: Considering growth and maturation indicators for a more tailored prediction approach for the youth demographic.

## References

- **Original Study**: "[Predicting youth diabetes risk using NHANES data and machine learning](https://doi.org/10.1038/s41598-021-90406-0)."
