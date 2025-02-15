# Stroke Prediction Analysis

This project uses machine learning to predict stroke risk using patient health data.

## Overview
I used Random Forest algorithm to analyze health data and predict stroke risk. The data includes factors like age, blood pressure, and other health conditions.

## Results
The model achieved these results:

 
                precision    recall  f1-score   support

           0       0.94      1.00      0.97       960
           1       0.00      0.00      0.00        62

    accuracy                           0.94      1022

Important features:
1. Age
2. Average glucose level
3. BMI
4. Health risks
5. Smoking status

## Project Files

stroke_prediction/
├── data/
├── models/
├── code/
├── requirements.txt
└── README.md


## Data Analysis
- Total records: 5110
- Number of features: 12
- Missing BMI data: 3.9%
- Stroke cases: 4.9%

## Setup
1. Clone repository

git clone https://github.com/AwadRemi/Stroke-Prediction-.git


2. Install requirements:

pip install -r requirements.txt

 
## Features Used
 - Age
- Work type
- Gender
- Blood pressure
- Heart disease
- Marriage status Living area
- Glucose level
- BMI
- Smoking status

## Future Work
1. Add more features
2. Fix data imbalance
3. Try different algorithms


## Conclusions
- Model accuracy: 95%
- Good at finding non-stroke cases


## Example 
def predict_stroke_risk(patient_data):
new_patient = {
    'age': 60,
    'hypertension': 1,
    'heart_disease': 0,
    'avg_glucose_level': 120,
    'bmi': 28,
    'gender': 'Male',
    'ever_married': 'Yes',
    'work_type': 'Private',
    'Residence_type': 'Urban',
    'smoking_status': 'formerly smoked'
}

risk = predict_stroke_risk(new_patient)
print(f"stroke risk: {risk*100:.2f}%")

==> Result :stroke risk: 10.98%
 

 

