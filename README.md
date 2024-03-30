# NHANES 2003-2004 Mortality Status Prediction

## Goal
This project aims to analyze the NHANES 2003-2004 dataset to predict the mortality status (binary outcome) of participants aged 50 years and older.

## Background
The National Health and Nutrition Examination Survey (NHANES) is a cross-sectional survey that is nationally representative and assesses demographic, dietary, and health-related questions. It is designed to understand health and nutrition differences across the lifespan. The National Center for Health Statistics (NCHS) makes almost all survey data publicly available.

## Dataset
The dataset for this project includes 813 variables covering various domains such as demographics, dietary intake, examination results, laboratory results, and questionnaire responses. Key domains include:
- Demographics (DEMO)
- Dietary Interview (DR1TOT, DR2TOT)
- Examination (BAX, BPX, BMX, CVX, VIX)
- Laboratory (L13AM, L13, L25, L11PSA)
- Questionnaire (ALQ, BPQ, DIQ, HSQ, MCQ, SSQ, WHQ)

Additionally, a 9-year follow-up mortality status from the NCHS linked mortality database is included.

### Key Variables
- `SEQN`: Respondent sequence number.
- `RIDAGEEX`: Age in months at the time of examination.
- `RIAGENDR`: Gender (1 = male, 2 = female).
- `BMXWT`: Weight in kg.
- `BMXHT`: Standing height in cm.
- `BMXBMI`: Body mass index (kg/m^2).
- `mortstat`: Final mortality status (0 = "Assumed alive", 1 ="Assumed Deceased").

## Problem Statement
Build a model to predict the mortality status (`mortstat`) for participants 50 years and older. Use sensitivity and specificity to determine the best model, and explain the choice between these two performance measures.

### Predictors
Explore and utilize the most informative predictors from the list provided, including but not limited to `RIDAGEYR`, `RIAGENDR`, `BMXBMI`, and several questionnaire and examination results.


## Resources
- [NHANES 2003-2004 Full Variable Descriptions](https://www.cdc.gov/nchs/nhanes/index.htm)
- [DEMO Component](https://wwwn.cdc.gov/nchs/nhanes/2003-2004/DEMO_C.htm)
- [MCQ Component](https://wwwn.cdc.gov/nchs/nhanes/2003-2004/MCQ_C.htm)

