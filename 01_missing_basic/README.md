# Missing Value Imputation Techniques – ML Mini Project

This repository focuses on understanding and applying different **missing value imputation techniques** using real-world datasets.  
The main objective of this project is **not model performance**, but to study how **mean, median, mode, and advanced imputation methods** work for different types of data.

---

## 1. Problem Statement

The goal of this project is to handle missing values in datasets using appropriate imputation techniques such as **mean, median, mode, KNN, and Iterative Imputer**, based on the nature of the data (numerical or categorical).

The project aims to:
- Understand the impact of missing values.
- Apply correct imputation strategies.
- Compare basic and advanced imputers.
- Visually verify the effect of imputation.

---

## 2. Approach

### Dataset 1: Diabetes Dataset
- Contains only **numerical features**.
- Missing values were handled using:
  - **Mean imputation**
  - **Median imputation**
  - **KNN Imputer**
  - **Iterative Imputer**
- `SimpleImputer`, `KNNImputer`, and `IterativeImputer` from scikit-learn were used.
- Models trained:
  - Random Forest
  - Decision Tree
- No outlier handling.
- No feature scaling.
- Purpose: Compare different imputation strategies on numerical data.

---

### Dataset 2: Ames Housing Dataset
- Contains both **numerical and categorical features**.
- Missing values were handled using:
  - **Median imputation** for numerical features (data is skewed).
  - **Mode imputation** for categorical features.
  - **"None"** for structural missing values (e.g., no garage, no pool).
  - **KNN Imputer** for selected numerical features.
  - **Iterative Imputer** for multivariate numerical imputation.
- No model training.
- Main focus: **Imputation techniques only**.
- Visual verification done using:
  - KDE plots for numerical features.
  - Bar plots for categorical features.
  - Before vs After comparison.

---

## 3. Key Learnings

- Mean and median are suitable for numerical data.
- Median is better for skewed distributions.
- Mode is best for categorical data.
- KNN Imputer uses similarity between samples.
- Iterative Imputer predicts missing values using other features.
- Structural missing values should be handled using domain knowledge.
- Imputation must always be fitted on training data only.
- Visual validation is important after imputation.

---

## 4. Tools Used

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Scikit-learn  

---

## 5. Conclusion

This project demonstrates how different imputation strategies should be applied based on data type and distribution.  
It also shows that **advanced imputers like KNN and Iterative Imputer can capture relationships between features**, leading to more realistic imputed values.

The focus is on **data preprocessing and missing value handling**, which is a critical step in any machine learning pipeline.
