# **Medical Adherence Lab: Predicting Medication Adherence**

## **Overview**

This project aims to predict medication adherence for patients with chronic diseases, specifically using data related to lifestyle factors, medical history, and socio-economic status. The goal is to build a model that can identify patients who are most likely to show low medication adherence based on various features.

## **Can a Random Forest Model Identify Low Medication Adherence?**

A **Random Forest** model is used to predict medication adherence based on various demographic, lifestyle, clinical, and symptom-related features. The model assesses the likelihood of a patient showing low adherence to medication and identifies patterns that may correlate with non-adherence.

### **Features Included in the Model**

#### **Demographics & Socio-economic**
- **Age**
- **Gender**
- **Ethnicity**
- **Socioeconomic Status**
- **Education Level**

#### **Lifestyle & Health Behaviors**
- **Smoking**
- **Alcohol Consumption**
- **Physical Activity**
- **Diet Quality**
- **Sleep Quality**

#### **Clinical Vitals & Laboratory Results**
- **BMI**
- **Systolic BP**
- **Diastolic BP**
- **Fasting Blood Sugar**
- **HbA1c**
- **Serum Creatinine**
- **BUN Levels**
- **Cholesterol Total**
- **Cholesterol LDL**
- **Cholesterol HDL**

#### **Chronic Conditions & History**
- **Family History Diabetes**
- **Gestational Diabetes**
- **Polycystic Ovary Syndrome**
- **Previous Pre-Diabetes**
- **Hypertension**
- **Diagnosis**

#### **Medications & Interventions**
- **Antihypertensive Medications**
- **Antidiabetic Medications**
- **Medication Adherence** (Target variable)

#### **Symptoms, Quality & Environment**
- **Frequent Urination**
- **Excessive Thirst**
- **Unexplained Weight Loss**
- **Blurred Vision**
- **Slow Healing Sores**
- **Fatigue Levels**
- **Tingling Hands/Feet**
- **Quality of Life Score**
- **Health Literacy**
- **Medical Checkups Frequency**
- **Heavy Metals Exposure**
- **Occupational Exposure Chemicals**
- **Water Quality Results**

## **Risk Score Classification**

In this project, patients are classified into two risk categories based on their **Medication Adherence Score**:

- **Low Risk**: Patients with a **score between 5.0 and 10.0** are considered low risk for non-adherence.
- **High Risk**: Patients with a **score between 0.0 and 5.0** are classified as high risk for non-adherence.

The model predicts these scores based on patient data, helping healthcare providers target high-risk individuals for interventions and support.

## **Results**

The model was evaluated on the test data, and after hyperparameter tuning, it showed the following performance metrics:
- **Precision**: 0.51
- **F1 Score**: 0.56
- **Recall**: 0.62

These results indicate that the model is effective in identifying patients who are more likely to show low medication adherence. The higher recall suggests that it is good at identifying more of the true non-adherent cases, while the precision indicates that some of the identified non-adherent cases are false positives.
