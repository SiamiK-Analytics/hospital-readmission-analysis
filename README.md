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



# Process phase using Xcel:Process Phase Presentation Script

After understanding the dataset during the Prepare phase, I moved into the Process phase.
The purpose of this phase was to ensure that the data was accurate, consistent, and ready for analysis.
I began by reviewing the dataset for missing values, duplicate records, invalid entries, and potential outliers. I also verified that numerical variables were correctly formatted as numbers and that categorical variables were consistently standardized.
Because the primary outcome of this project is 30-day hospital readmission, I carefully validated the Readmitted_Within_30_Days variable to ensure that the outcome was consistently coded as zero for patients who were not readmitted and one for patients who were readmitted.
I also reviewed binary variables such as ICU_Stay_Flag, High_Risk_Medication_Flag, and Followup_Appointment_Scheduled to ensure that their values were consistently coded.
Finally, I transformed selected variables into analytical categories, such as age groups, previous admission groups, and chronic disease burden categories. These transformations made it easier to identify patterns and compare readmission rates across different patient populations.
After completing these steps, I had a clean and structured dataset that was ready for deeper analysis using SQL, Python, and Tableau.
  
📊 What Your Process Phase Can Look Like

PROCESS: Cleaning and Preparing the Data

-Step 1 — Data Quality Checks

-Checked for missing values

-Identified duplicate records

-Reviewed invalid values

-Investigated outliers

Step 2 — Data Standardization

-Standardized categorical variables

-Verified binary variables

-Confirmed numeric data types

Step 3 — Data Transformation

-Created analytical categories

-Prepared variables for SQL analysis

-Prepared data for Python analysis

-Structured fields for Tableau visualizations

Step 4 — Validation

-Confirmed the target variable was correctly coded

-Verified that the final dataset was analysis-ready

🔥 Strong Transition to the Analyze Phase

End your Process section with:

“Once the data had been cleaned, standardized, and validated, I was ready to move into the Analyze phase and begin investigating which factors were most strongly associated with 30-day hospital readmission.”




# Analyse phase with Xcel,SQL, Python:

🎯 Analyze Phase Objective

The objective of the Analyze phase was to examine patterns and relationships within the patient data to determine which demographic, clinical, healthcare utilization, medication, and discharge-related factors were associated with 30-day hospital readmission.

****Your Analyze Phase Presentation Script

After cleaning and validating the dataset, I moved into the Analyze phase.

The purpose of this phase was to identify patterns and relationships between patient characteristics and 30-day hospital readmission.

I began by calculating the overall readmission rate to establish a baseline for the analysis. From there, I examined several categories of potential factors, including previous healthcare utilization, clinical complexity, medication management, post-discharge care, demographics, and socioeconomic risk.

First, I analyzed whether patients with a history of previous admissions or readmissions had different readmission rates compared with patients who had less prior hospital utilization.

Next, I examined clinical complexity by looking at comorbidity burden, chronic disease count, severity score, and ICU stays.
I also analyzed medication-related factors, including the number of medications, medication changes, high-risk medications, and medication adherence.

Because the transition from hospital to home may be important, I examined whether follow-up appointments and discharge disposition were associated with different readmission outcomes.

Finally, I compared readmission rates across demographic and socioeconomic factors, including age, gender, insurance type, and socioeconomic risk score.

The goal of this phase was not simply to identify differences between groups, but to determine which patterns appeared most strongly associated with 30-day readmission and could provide meaningful insights for healthcare decision-making.

# 🔥 How to Make Your Analyze Phase Stand Out
Don't simply say:

“Patients with X had a higher readmission rate.”

Instead, present each finding like this:

Finding

What did the data show?

Does the analysis show association or causation?

For example:

Finding: Patients with previous readmissions had a higher 30-day readmission rate than patients without previous readmissions.

Interpretation: This suggests that prior hospital utilization may be an important indicator of future readmission risk.
Caution: This relationship is associative and does not prove that previous readmissions directly cause future readmissions.


🎯 Your Analyze Phase Transition

End the section with:

“After analyzing these factors, I identified the strongest patterns associated with 30-day readmission. The next step was to translate those findings into clear visualizations and communicate the insights to healthcare stakeholders.”
That leads perfectly into your SHARE phase, where you can present your Tableau dashboard and key findings.



# Share phase with  and Tableau or Power BI:
# Act phase or Recommendations:
