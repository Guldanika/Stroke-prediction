# Stroke Prediction Project

## Project Overview
This project aims to develop a machine learning model to predict the likelihood of stroke based on patient data. The primary objective is to identify all potential stroke cases, with a strong focus on maximizing sensitivity (recall) to ensure no stroke cases are missed. This project uses real-world-inspired healthcare data, making it applicable for practical use in early diagnosis and prevention strategies.

## Motivation
Stroke is a leading cause of death and disability worldwide. Early detection can significantly improve patient outcomes by enabling timely intervention. This project seeks to leverage data science to assist healthcare professionals in identifying high-risk patients and potentially saving lives.

## Dataset
The dataset used for this project contains the following features:
- **id**: Unique identifier for each patient.
- **gender**: Gender of the patient.
- **age**: Age of the patient.
- **hypertension**: Whether the patient has hypertension (0 = No, 1 = Yes).
- **heart_disease**: Whether the patient has heart disease (0 = No, 1 = Yes).
- **ever_married**: Marital status of the patient (Yes/No).
- **avg_glucose_level**: Average glucose level in the blood.
- **bmi**: Body Mass Index of the patient.
- **stroke**: Target variable indicating if the patient had a stroke (0 = No, 1 = Yes).
- **Additional Features**: Derived and encoded variables, including:
  - **bmi_hypertension**: Interaction term between BMI and hypertension.
  - **bmi_glucose**: Interaction term between BMI and glucose level.
  - **smoking_status_numeric**: Numerical encoding of smoking status.
  - **bmi_smoking**: Interaction term between BMI and smoking status.
  - **bmi_cat**, **age_cat**, **glucose_cat**: Categorical groupings of BMI, age, and glucose levels.
  - **work_type**: One-hot encoded work categories (e.g., Private, Self-employed).
  - **smoking_status**: One-hot encoded smoking categories (e.g., smokes, formerly smoked).
  - **Residence_type**: Urban or rural residence.

## Methodology
1. **Data Preprocessing**:
   - Handled missing values in features like BMI and glucose levels.
   - Scaled continuous variables to ensure uniformity.
   - One-hot encoded categorical variables.
   - Engineered interaction terms and grouped features for better representation.

2. **Exploratory Data Analysis (EDA)**:
   - Explored feature distributions and their correlation with stroke occurrences.
   - Analyzed imbalances in the target variable.

3. **Model Development**:
   - Tried various classification models such as Logistic Regression, Random Forest, and Gradient Boosting.
   - Focused on hyperparameter tuning to improve model performance.
   - Applied techniques like SMOTE to address class imbalance.

4. **Evaluation Metrics**:
   - Sensitivity (Recall): Priority metric to minimize false negatives.
   - Precision, F1-score, and ROC-AUC for a comprehensive evaluation.

## Results
- Achieved a high recall score to ensure the majority of stroke cases were correctly identified.
- Improved model performance by incorporating feature engineering and addressing class imbalance.

## Challenges
- Handling imbalanced data was a significant challenge due to the low prevalence of stroke cases in the dataset.
- Balancing sensitivity with precision required careful selection of thresholds.

## Future Work
- Incorporate additional features such as patient history and genetic predisposition.
- Deploy the model as an API for real-time predictions.
- Evaluate the model on external datasets to assess generalizability.


---

Feel free to contribute to this project or reach out with any feedback or suggestions!


