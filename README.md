Healthcare Data Cleaning and Visualization

This project demonstrates how to clean, preprocess, and visualize a sample healthcare dataset using Python and key libraries like pandas, numpy, and matplotlib.

Dataset Overview

The dataset includes the following columns:

PatientID: Unique identifier for each patient

Age: Age of the patient (years)

BloodPressure: Blood pressure readings (mmHg)

SugarLevel: Blood sugar levels (mg/dL)

Weight: Patient weight (kg)

Steps for Data Cleaning

1. Handling Missing Values

Checked for missing values using data.isnull().sum().

If any were present, appropriate methods such as filling numerical data with the median or categorical data with the mode would be applied. However, no missing values were found in this dataset.

2. Handling Duplicates

Duplicates were checked using data.duplicated().sum().

Any duplicate rows were removed using data.drop_duplicates().

3. Data Normalization

Min-Max scaling was applied to the numerical columns (Age, BloodPressure, SugarLevel, and Weight) to bring values into a 0-1 range.

This improves model performance and ensures fair feature comparison.
