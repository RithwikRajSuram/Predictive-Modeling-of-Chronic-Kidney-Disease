# Chronic Kidney Disease Prediction using Random Forest

## Project Overview
This project uses machine learning to predict whether a patient is likely to have Chronic Kidney Disease (CKD) based on clinical and diagnostic health indicators. A Random Forest classification model was trained on kidney disease data and used to classify patients as either `ckd` or `notckd`.

The project focuses on healthcare data preprocessing, model training, prediction, accuracy evaluation, and feature importance analysis. This makes it a strong portfolio project for healthcare analytics, health data science, and machine learning roles.

## Objective
The main objective of this project is to build a classification model that can support early identification of Chronic Kidney Disease using patient health variables such as blood pressure, serum creatinine, albumin, blood glucose, hypertension, diabetes status, and other clinical features.

## Dataset
The dataset contains patient-level clinical records related to kidney disease. Each row represents a patient record with demographic, laboratory, and medical condition variables.

### Example Columns
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

## Tools and Libraries Used
- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Random Forest Classifier

 ## Model Evaluation

The model achieved the following accuracy:

Random Forest Accuracy: 85.71%

This means the model correctly classified approximately 86% of the patient records in the evaluated test set.

## Feature Importance Analysis

Random Forest feature importance was used to identify which variables had the strongest impact on the model prediction.

In this analysis, the most important features were:

Feature	Interpretation
sc	Serum creatinine had the highest importance and was the strongest predictor in the model
bp	Blood pressure also contributed to CKD prediction
Results

The Random Forest model produced strong classification performance with an accuracy of 85.71%.

The feature importance chart showed that:

Serum creatinine (sc) was the most influential variable in predicting CKD.
Blood pressure (bp) also contributed to the prediction outcome.
The model successfully generated CKD predictions for unseen patient records.
Key Visualization
Random Forest Feature Importance

The feature importance chart highlights the clinical variables that contributed most to the Random Forest prediction model.

## Conclusion

This project demonstrates the use of machine learning in healthcare analytics to classify Chronic Kidney Disease risk from clinical data. The Random Forest model achieved an accuracy of 85.71%, and feature importance analysis showed serum creatinine as the strongest predictor, supporting the value of data-driven approaches in early disease detection.
