# Chronic Kidney Disease Prediction using Random Forest

## Project Overview
This project uses machine learning to predict whether a patient is likely to have Chronic Kidney Disease (CKD) based on clinical and diagnostic health indicators. A Random Forest classification model was trained on kidney disease data and used to classify patients as either `ckd` or `notckd`.

The project focuses on healthcare data preprocessing, model training, prediction, accuracy evaluation, and feature importance analysis. This makes it a strong portfolio project for healthcare analytics, health data science, and machine learning roles.

## Objective
The main objective of this project is to build a classification model that can support early identification of Chronic Kidney Disease using patient health variables such as blood pressure, serum creatinine, albumin, blood glucose, hypertension, diabetes status, and other clinical features.

## Dataset
The dataset contains patient-level clinical records related to kidney disease. Each row represents a patient record with demographic, laboratory, and medical condition variables.

## Example Columns
- `age` - Patient age
- `bp` - Blood pressure
- `sg` - Specific gravity
- `al` - Albumin
- `su` - Sugar
- `rbc` - Red blood cells
- `pc` - Pus cell
- `pcc` - Pus cell clumps
- `ba` - Bacteria
- `bgr` - Blood glucose random
- `bu` - Blood urea
- `sc` - Serum creatinine
- `sod` - Sodium
- `pot` - Potassium
- `hemo` - Hemoglobin
- `pcv` - Packed cell volume
- `wc` - White blood cell count
- `rc` - Red blood cell count
- `htn` - Hypertension
- `dm` - Diabetes mellitus
- `cad` - Coronary artery disease
- `appet` - Appetite
- `pe` - Pedal edema
- `ane` - Anemia
- `classification` - CKD status

## Considered Factors
For this Random Forest model, the analysis focused on the following clinical features:

- `bp` - Blood pressure  
- `sc` - Serum creatinine  

These two variables were used as the main input features for predicting whether a patient is classified as `ckd` or `notckd`.

## Tools and Libraries Used
- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Random Forest Classifier

## Model Evaluation
Logistic Regression Confusion Matrix

The Logistic Regression model produced the following confusion matrix:

Actual / Predicted	Non-CKD	CKD
Non-CKD	18	4
CKD	5	25
Confusion Matrix Interpretation
18 non-CKD patients were correctly classified as non-CKD.
25 CKD patients were correctly classified as CKD.
4 non-CKD patients were incorrectly classified as CKD.
5 CKD patients were incorrectly classified as non-CKD.

This shows that the Logistic Regression model performed well in identifying CKD cases while maintaining a reasonable balance between false positives and false negatives.

## ROC Curve and AUC

The Logistic Regression model achieved an AUC score of:

AUC = 0.92

An AUC of 0.92 indicates strong classification performance and shows that the model was able to separate CKD and non-CKD patients effectively.

## Random Forest Accuracy

The Random Forest model achieved an accuracy of:

Random Forest Accuracy = 85.71%

This means the model correctly classified approximately 86% of the evaluated patient records.

## Visualizations
Linear Regression: Serum Creatinine vs Blood Pressure

This plot shows the relationship between blood pressure and serum creatinine. The regression line indicates a slight positive association between the two variables.

ROC Curve - Logistic Regression

The ROC curve shows the trade-off between true positive rate and false positive rate. The model achieved an AUC of 0.92, indicating strong classification performance.

Confusion Matrix - Logistic Regression

The confusion matrix shows how many CKD and non-CKD patients were correctly and incorrectly classified by the Logistic Regression model.

Random Forest Feature Importance
The Random Forest feature importance chart shows which selected clinical variables contributed most to CKD prediction.

## Key Findings
Logistic Regression performed strongly in distinguishing CKD and non-CKD patients.
The ROC-AUC score of 0.92 indicates strong classification ability.
Random Forest achieved an accuracy of 85.71%.
Serum creatinine was the most important predictor in the Random Forest model.
Blood pressure also contributed to CKD prediction.
Linear Regression showed a slight positive relationship between blood pressure and serum creatinine.

## Conclusion

This project demonstrates how machine learning can be applied to healthcare data to support Chronic Kidney Disease risk classification. Logistic Regression showed strong classification performance with an AUC of 0.92, while Random Forest achieved 85.71% accuracy and identified serum creatinine as the strongest predictor among the selected features.
