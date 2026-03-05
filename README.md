# Student Performance Classification using Machine Learning

A machine learning project that investigates the relative influence of family background vs. school environment on student academic success using classification models. Built using Python and Scikit-learn on real student performance datasets.

## Research Question

Which has a greater impact on student academic success — family background or school environment?

## Dataset

Two publicly available datasets were used: `student-mat.csv` (Mathematics) and `student-por.csv` (Portuguese), tracking student performance in secondary school. The final grade (G3) was transformed into a binary classification target (pass/fail).

Features were divided into two conceptual groups:
- **Family background** — parental education, parental occupation, family relationship quality, guardian type
- **School environment** — absences, study time, academic support, school-related activities

## Tech Stack

- **Language:** Python
- **Libraries:** Scikit-learn, Pandas, NumPy, Matplotlib
- **Models:** Logistic Regression, Random Forest, SVM

## Methodology

- Features split into three experimental configurations: family-only, school-only, and combined
- Categorical variables encoded using one-hot encoding; numerical features normalized
- Stratified train/test split to preserve class balance
- Hyperparameter tuning via grid search with cross-validation
- PCA applied separately to family and school feature sets for visualization

## Key Findings

- **Mathematics dataset:** School-related features (especially absences and study time) yielded the highest F1-scores, with Random Forest performing best using school-only features.
- **Portuguese dataset:** Family background features achieved the highest F1-scores; school-only models underperformed comparatively.
- **Feature importance:** Within the family group, parental education, parental occupation, and family relationship quality were most influential.
- **PCA:** School feature sets provided more geometrically separable class distributions despite family features explaining a comparable proportion of variance.
- **Overall:** Results suggest school environment factors are stronger predictors for Mathematics, while family background plays a more meaningful role in Portuguese performance.

## Model Evaluation

Models were evaluated using accuracy, precision, recall, and F1-score. F1-score was emphasized as the primary metric to handle class imbalance. Confusion matrix analysis showed that family-only models tended toward different misclassification patterns compared to school-only models.

## Setup

1. Clone the repository
2. Install dependencies:
   ```bash
   pip install scikit-learn pandas numpy matplotlib
   ```
3. Run the preprocessing script, then train and evaluate the models.

## Authors

Beyzanur Deniz, Can Eye, Gizem Uluceviz, Özgür Akyol  
Management Information Systems, Kadir Has University — MIS325 Data Mining & Business Intelligence
