# Student Academic Success Prediction

This project analyzes the impact of **family background** and **school environment** factors on student academic success using machine learning models.

---

## Project Objective

The main objective of this project is to compare the predictive power of:

- **Family-related features**
- **School-related features**

in determining student academic success.

The analysis focuses on identifying which factors are more influential depending on the subject.

---

## Dataset

Two public educational datasets were used:

- `student-mat.csv` – Mathematics dataset  
- `student-por.csv` – Portuguese language dataset  

The datasets include:

- demographic information  
- family background variables  
- school environment characteristics  
- student grades  

### Academic Success Definition

- **G3 ≥ 10** → Successful  
- **G3 < 10** → Unsuccessful  

---

## Data Preprocessing

The following preprocessing steps were applied:

- One-hot encoding for categorical variables  
- Standardization using z-score normalization  
- Stratified train-test split to preserve class distribution  

---

## Machine Learning Models

The following classification models were used:

- Logistic Regression  
- Random Forest  
- Support Vector Machine (SVM)  

---

## Dimensionality Reduction

Principal Component Analysis (**PCA**) was applied to visualize the separation between successful and unsuccessful students based on feature groups.

---

## Evaluation Metrics

Model performance was evaluated using:

- Accuracy  
- Precision  
- Recall  
- F1-score  

The **F1-score** was emphasized because it balances precision and recall in binary classification problems.

---

## Key Findings

- **School-related variables** such as absences and study time showed stronger predictive power for **Mathematics performance**.  
- **Family background variables** were slightly more influential for **Portuguese language performance**.  
- Combining both feature groups did not significantly improve prediction performance.

These findings suggest that different subjects may be influenced by different contextual factors.

---
