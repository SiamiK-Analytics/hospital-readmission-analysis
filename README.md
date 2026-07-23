# HOSPITAL-READMISSION-ANALYSIS: reducing Hospital Readmissions Through Data Analytics

## Introduction
Imagine a patient being discharged from the hospital after receiving treatment. The hospital considers the stay complete, but for the patient, the recovery process has only just begun.

Within the next 30 days, that patient may return to the hospital.

The question is: **Could data help us identify which patients may be at higher risk before that readmission happens?**

That question is the foundation of my capstone project, **Hospital Readmission Risk Analysis**.

Using 18,000 patient records, I analyzed clinical history, previous admissions, chronic conditions, severity of illness, medication changes, medication adherence, follow-up care, and discharge information.

My objective was to move beyond simply describing what happened. I wanted to discover patterns, identify potential risk factors, and translate those findings into insights that could support better healthcare decision-making.

Through Excel, SQL, Python, and Tableau, this project demonstrates how a data analyst can transform healthcare data into a clearer understanding of readmission risk.


## Ask Phase 
Primary stakeholders:

-Hospital administrators

-Clinical care teams

-Case managers

-Discharge planners

-Quality improvement teams

-Healthcare analysts

#### Their business question:

How can we use patient data to better understand readmission patterns and identify opportunities to improve post-discharge support?

# I recommend presenting your Ask phase like this:
# Defining the Problem
# Healthcare Challenge:
Some patients return to the hospital within 30 days of discharge, potentially indicating a need for additional support during the transition from hospital to home.
Analytical Question:
What patient, clinical, medication, utilization, and discharge-related factors are associated with 30-day hospital readmission?
Project Objective:
To analyze 18,000 patient records and identify patterns associated with 30-day readmission outcomes, using data analytics to generate actionable insights that could help healthcare organizations better understand high-risk patient populations and improve post-discharge care strategies.
Expected Value:
By identifying important patterns in readmission data, this analysis can help healthcare stakeholders better understand where additional patient support and follow-up may be most valuable.

🎤 What you can say out loud
“After framing the problem, I moved into the Ask phase of my analysis. The central question I wanted to answer was: What factors are associated with a patient being readmitted within 30 days of discharge? My objective was to analyze 18,000 patient records and examine clinical history, previous hospital utilization, chronic conditions, medication-related factors, follow-up care, and discharge information. The goal was not to predict an individual patient's outcome or replace clinical judgment, but to identify meaningful patterns in the data that could help healthcare organizations better understand readmission risk and opportunities for improved post-discharge support.”

###### ###Important: I recommend using the phrase “associated with readmission” rather than saying your analysis proves that a factor causes readmission. That makes your project more statistically accurate and professionally credible.#####

# Key Questions for Your Analysis
### Primary Question:
-What factors are most strongly associated with a patient's likelihood of being readmitted within 30 days of discharge?
### Supporting Questions:
-Do patients with more previous hospital admissions have higher readmission rates?

-How does the number of chronic conditions relate to readmission risk?

-Are patients with longer hospital stays more likely to be readmitted?

-Does medication adherence appear to be associated with readmission outcomes?

-Is a follow-up appointment after discharge associated with lower readmission rates?

-How do ICU stays and illness severity relate to readmission risk?

-Are there differences in readmission rates across age groups or other demographic categories?

-Are medication changes during hospitalization associated with different readmission outcomes?



# Prepare phase using Kaggle:

The objective of the Prepare phase was to assess, organize, and validate the dataset to ensure that the patient records and variables were complete, consistent, and suitable for analyzing factors associated with 30-day hospital readmission.

After defining the business problem and analytical questions, I moved into the Prepare phase.
The dataset used in this project contains 18,000 patient records and 25 variables related to demographics, previous healthcare utilization, clinical conditions, laboratory measurements, medications, follow-up care, and discharge outcomes.
The primary outcome variable for this analysis is Readmitted_Within_30_Days, which identifies whether a patient was readmitted within 30 days of discharge.
Before beginning the analysis, I organized the variables into logical categories to better understand how each group could relate to readmission risk. These categories included patient demographics, previous hospital utilization, clinical severity, chronic disease burden, medication-related factors, follow-up care, and discharge information.
I also assessed the dataset for data quality issues, including missing values, duplicate records, inconsistent data types, invalid values, and potential outliers.
The goal of this phase was to ensure that the data was reliable, structured, and ready for analysis. Establishing a clean and well-understood dataset was important because the quality of the analysis depends on the quality of the data being analyzed.

### Slide Title: Prepare — Understanding the Data

Dataset:

--18,000 patient records

--25 variables

--CSV format

Data Domains:

--Demographics

--Healthcare utilization

--Clinical conditions

--Laboratory measurements

--Medications

--Follow-up care

--Discharge outcomes

Target Variable:

-Readmitted_Within_30_Days

Data Preparation Goals:

--Validate data types

--Identify missing values

--Check duplicates

--Review outliers

--Standardize categorical variables

--Confirm target variable coding

🔥 Strong transition into the Process phase
End your Prepare section with:
“Once I understood the structure and quality of the dataset, the next step was to clean and transform the data so it could be analyzed consistently across Excel, SQL, Python, and Tableau.”

****extra to know or consider:
Understanding the Dataset Structure

Your dataset contains variables that can be organized into analytical categories:

👤 Demographic Variables

---Age

--Gender

--Insurance_Type

--Socioeconomic_Risk_Score

🏥 Previous Healthcare Utilization

--Previous_Admissions_6M

--Previous_Readmissions_1Y

--Time_Since_Last_Discharge

🩺 Clinical and Disease Burden

--Primary_Diagnosis_Group

--Comorbidity_Index

--Chronic_Disease_Count

--Severity_Score

--ICU_Stay_Flag

🧪 Clinical Measurements

--HbA1c_Level

--Creatinine_Level

--Hemoglobin_Level

--Average_Systolic_BP

💊 Medication Factors

--Number_of_Medications

--Medication_Change_Count

--High_Risk_Medication_Flag

--Medication_Adherence_Score

📅 Discharge and Follow-Up

--Followup_Appointment_Scheduled
--Discharge_Disposition

🎯 Target Variable

--Readmitted_Within_30_Days

This categorization is important because it connects directly to your research questions.

