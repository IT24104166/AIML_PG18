# AIML_PG18
Group project for AI/ML preprocessing pipeline
Project Overview

This project focuses on data preprocessing and exploratory data analysis (EDA) for the Diabetes Readmission Dataset.
The aim is to prepare the dataset for machine learning by ensuring data quality, consistency, and usability.

Pipeline covers all essential steps:

Handling Missing Data (IT24104212 – Yapa S.K.S.)

Identified missing values and placeholders (e.g., “?”, “Unknown/Invalid”).
Replaced or imputed missing values using appropriate strategies (median for numeric, mode for categorical).

Encoding Categorical Variables (IT24104154 – Indunil D.G.T.)

Converted categorical variables (e.g., gender, race, admission type) into machine-readable numeric form.
Applied label encoding and one-hot encoding where appropriate.

Outlier Removal (IT24104232 – Sarvithan P.)

Detected outliers using statistical methods (IQR and z-score).
Applied removal/replacement to reduce noise and improve data quality.

Feature Engineering (IT24104201 – Anupadha H.M.I.)

Created new features from existing ones to improve predictive power.
Example: deriving numeric midpoint from age ranges, grouping diagnosis codes.

Normalization (IT24104234 – Dhanujaya G.D.I.T.)

Scaled numeric features to a standard range (MinMaxScaler, StandardScaler).
Ensured all features are comparable for model training.

Data Cleaning & EDA (IT24104166 – Kumarasegaran D.)

Removed duplicates, standardized data types, and audited missing values.
Conducted exploratory analysis with visualizations (histograms, boxplots, bar charts, scatter plots, correlation heatmap).
Generated an IQR-based outlier report for transparency.


 Dataset Details

Dataset: Diabetes Readmission Dataset
Source: UCI Machine Learning Repository
Size: ~100,000 patient records, 50 features
Contents: Demographics, hospital visits, diagnoses, lab results, medications, and readmission status


Group Members & Roles

| Student ID | Name               | Assigned Role                  |
| ---------- | ------------------ | ------------------------------ |
| IT24104166 | Kumarasegaran D.   | Data Cleaning & EDA            |
| IT24104201 | Anupadha H.M.I.    | Feature Engineering            |
| IT24104212 | Yapa S.K.S.        | Handling Missing Data          |
| IT24104234 | Dhanujaya G.D.I.T. | Normalization                  |
| IT24104232 | Sarvithan P.       | Outlier Removal                |
| IT24104154 | Indunil D.G.T.     | Encoding Categorical Variables |


How to Run the Code

1.Clone or download this repository.
2.Place the dataset inside:data/raw/diabetic_data.csv
3.Open the individual notebooks from the notebooks/ folder to view each member’s preprocessing technique:
     ITxxxxxxx_Preprocessing_technique.ipynb
4.Run the combined pipeline notebook:
  group_pipeline.ipynb → integrates all preprocessing steps into one flow.
5.All results will be saved in:
  results/eda_visualizations/ → plots & charts (PNG/JPEG)
  results/outputs/ → cleaned datasets & processed outputs
  results/logs/ → logs (optional)
