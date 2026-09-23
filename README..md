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

## Key Findings

### Academic Performance

Average scores across the three subjects:

| Subject | Average Score |
|---|---:|
| Math | 66.69 |
| Reading | 69.44 |
| Writing | 68.45 |

Reading has the highest average score, while Math has the lowest.

### Parental Education

Parental education shows a clear relationship with academic performance.

Students whose parents hold a Master's Degree recorded higher average scores than students whose parents completed only Some High School.

| Parental Education | Math | Reading | Writing |
|---|---:|---:|---:|
| Master's Degree | 72.49 | 76.17 | 76.86 |
| Bachelor's Degree | 70.55 | 73.16 | 73.45 |
| Associate's Degree | 68.66 | 71.44 | 70.55 |
| Some College | 66.51 | 68.91 | 68.19 |
| High School | 64.26 | 67.04 | 65.08 |
| Some High School | 62.81 | 65.81 | 63.93 |

The gap between the highest and lowest parental-education groups ranges from **9.7 points in Math to 12.9 points in Writing**.

### Parental Marital Status

The analysis found relatively small differences across parental marital-status groups.

Math scores range from approximately **66.1 to 69.4** across the four groups, a spread of about **3.3 points**.

### Data Quality

The dataset contains **11,040 records across 15 columns**.

Overall cell completeness is approximately **96.9%**.

The largest missing-data gaps occur in:

- **TransportMeans — 89.67% complete**
- **EthnicGroup — 93.98% complete**
- **TestPrep — 94.03% complete**
- **ParentEduc — 94.04% complete**

The three main score fields are essentially complete.

## Important Analytical Limitation

Several variables were collected in the dataset but were **not analysed against academic scores in the source notebook**.

These include:

- `TestPrep`
- `WklyStudyHours`
- `PracticeSport`
- `LunchType`
- `TransportMeans`
- `NrSiblings`
- `IsFirstChild`

Therefore, this project does **not** claim that these variables do or do not affect academic performance.

They represent **opportunities for future analysis**.

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
