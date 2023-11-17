# Glioma Grade Classification Project

## Introduction
The goal of this project is to develop a machine learning model capable of accurately detecting the grade of glioma in individuals. 
Gliomas are a type of brain tumor, and accurately identifying the grade is crucial for determining the appropriate treatment for patients. 
The target variable in this project is the glioma grade, with two classes: "LGG" (Low-Grade Glioma) and "GBM" (Glioblastoma Multiforme).

In order to carry this project, we are going to use dataset from 'Hierarchical Voting-Based Feature Selection and Ensemble Learning Model Scheme 
for Glioma Grading with Clinical and Molecular Characteristics By E. Tasci, Y. Zhuge, Harpreet Kaur, K. Camphausen, A. Krauze. 2022'. 
The author managed to get 87.606% using 20.5 (mean) number of features. By the end of this project, we found out that our KNN model managed to get to 87.8% accuracy 
by only using 5 features.

## Dataset Features

### Demographic Information

- **Grade (Target):** Glioma grade class information. (*LGG*, *GBM*-->*0*,*1*)
- **Gender:** Gender information. (*MALE*, *FEMALE*)
- **Age at Diagnosis:** Age at diagnosis measured in years.
- **Race:** Race information.

### Molecular Mutation Status

- **IDH1:** Isocitrate dehydrogenase 1 mutation status (*NOT_MUTATED*, *MUTATED*).
- **TP53:** Tumor protein p53 mutation status (*NOT_MUTATED*, *MUTATED*).
- **ATRX:** ATRX chromatin remodeler mutation status (*NOT_MUTATED*, *MUTATED*).
- **PTEN:** Phosphatase and tensin homolog mutation status (*NOT_MUTATED*, *MUTATED*).
- **EGFR:** Epidermal growth factor receptor mutation status (*NOT_MUTATED*, *MUTATED*).
- **CIC:** Capicua transcriptional repressor mutation status (*NOT_MUTATED*, *MUTATED*).
- **MUC16:** Mucin 16 mutation status (*NOT_MUTATED*, *MUTATED*).
- **PIK3CA:** Phosphatidylinositol-4,5-bisphosphate 3-kinase catalytic subunit alpha mutation status (*NOT_MUTATED*, *MUTATED*).
- **NF1:** Neurofibromin 1 mutation status (*NOT_MUTATED*, *MUTATED*).
- **PIK3R1:** Phosphoinositide-3-kinase regulatory subunit 1 mutation status (*NOT_MUTATED*, *MUTATED*).
- **FUBP1:** Far upstream element binding protein 1 mutation status (*NOT_MUTATED*, *MUTATED*).
- **RB1:** RB transcriptional corepressor 1 mutation status (*NOT_MUTATED*, *MUTATED*).
- **NOTCH1:** Notch receptor 1 mutation status (*NOT_MUTATED*, *MUTATED*).
- **BCOR:** BCL6 corepressor mutation status (*NOT_MUTATED*, *MUTATED*).
- **CSMD3:** CUB and Sushi multiple domains 3 mutation status (*NOT_MUTATED*, *MUTATED*).
- **SMARCA4:** SWI/SNF related, matrix associated, actin-dependent regulator of chromatin, subfamily a, member 4 mutation status (*NOT_MUTATED*, *MUTATED*).
- **GRIN2A:** Glutamate ionotropic receptor NMDA type subunit 2A mutation status (*NOT_MUTATED*, *MUTATED*).
- **IDH2:** Isocitrate dehydrogenase (NADP(+)) 2 mutation status (*NOT_MUTATED*, *MUTATED*).
- **FAT4:** FAT atypical cadherin 4 mutation status (*NOT_MUTATED*, *MUTATED*).
- **PDGFRA:** Platelet-derived growth factor receptor alpha mutation status (*NOT_MUTATED*, *MUTATED*).

### Additional Information

- **Project:** Corresponding TCGA-LGG or TCGA-GBM project names.
- **Case_ID:** Related project Case_ID information.
- **Primary_Diagnosis:** Type of primary diagnosis information.

## Procedures
1. Data Preprocessing
   -Importing Data
   -Exploratory Data Analysis
   -Encoding
   -Imputation
   -Min-Max Scaling
   -Dropping unimportant Features
2. Hyperparameter Tuning and Modeling
   -Logistic Regression
   -K-Nearest Neighbors
   -Naive Bayes
   -Support Vector Machine
3. Model Comparison
   -Accuracy
   -Learning Curve
   -Classification Report

**Note: Please refer to requirements.txt for dependencies. I used numpy 1.23.5 for this project. Most of other version including 1.24 above seem to cause errors/**
