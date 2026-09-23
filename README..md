# Student Performance Analytics

A Python-based exploratory data analysis project examining academic performance across 11,040 students and identifying patterns related to demographics and family background.

## Project Overview

This project analyzes student performance using Math, Reading, and Writing scores along with demographic and family-background variables.

The analysis focuses on:

- Academic score distributions
- Gender and ethnic-group composition
- Parental education
- Parental marital status
- Missing-data and data-quality assessment
- Group-wise academic performance comparisons
- Identification of areas for further analysis

## Business / Analytical Questions

1. How are Math, Reading, and Writing scores distributed?
2. What is the demographic composition of the student cohort?
3. How does parental education relate to academic performance?
4. Does parental marital status show a meaningful relationship with scores?
5. Which variables have missing data?
6. Which collected variables require further analysis?

## Dataset

**Dataset:** `Expanded_data_with_more_features.csv`

The dataset contains **11,040 student records** and 15 columns.

### Main outcome variables

- MathScore
- ReadingScore
- WritingScore

### Demographic and background variables

- Gender
- EthnicGroup
- ParentEduc
- ParentMaritalStatus
- TestPrep
- WklyStudyHours
- PracticeSport
- LunchType
- TransportMeans
- NrSiblings
- IsFirstChild

The `Unnamed: 0` index column was identified as a data-loading artefact and removed during analysis.

## Tools & Technologies

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Exploratory Data Analysis
- Data Cleaning
- Data Visualization
- Group-wise Analysis

## Analysis Workflow

```text
Raw Dataset
     ↓
Data Loading
     ↓
Data Quality & Missing-Value Analysis
     ↓
Data Cleaning
     ↓
Exploratory Data Analysis
     ↓
Group-wise Performance Analysis
     ↓
Visualization
     ↓
Insights & Recommendations
