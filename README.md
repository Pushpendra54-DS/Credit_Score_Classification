# Credit Score Classification
A machine learning project to predict customer credit scores (Good, Standard, Poor) using classification models such as Logistic Regression, Decision Tree, and Random Forest. Includes data preprocessing, outlier detection, feature selection using VIF, and model evaluation.

## Table of Contents
1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Data Preprocessing](#data-preprocessing)
4. [Exploratory Data Analysis](#exploratory-data-analysis)
5. [Feature Selection](#feature-selection)
6. [Model Building](#model-building)
7. [Results](#results)
8. [Conclusion](#conclusion)
9. [Future Work](#future-work)

## Project Overview
This project aims to predict the credit score category of customers based on various financial and demographic factors. 
The dataset contains 100,000 records with 28 features, including information about income, debt, payment history, credit mix, and more.

The workflow includes:
- Data cleaning and preprocessing
- Handling missing values using forward and backward filling
- Outlier detection and removal
- Encoding categorical variables using One-Hot Encoding
- Feature selection using Variance Inflation Factor (VIF)
- Model building with Logistic Regression, Decision Tree, and Random Forest
- Hyperparameter tuning using GridSearchCV
- Model evaluation using accuracy score, confusion matrix, and other metrics

## Dataset
- Source: (Add your dataset link if public or mention it's confidential/sample data)
- Number of Records: 100,000
- Number of Features: 28
- Target Variable: `Credit_Score` (Good / Standard / Poor)
- Feature Types: Numerical and Categorical

## Data Preprocessing
- Removed unnecessary columns
- Replaced special characters (`_` or `NM`) with null values or meaningful replacements
- Converted categorical features into numerical values using Label Encoding / One-Hot Encoding
- Filled missing values using forward and backward fill methods
- Removed outliers from `Age` column
- Standardized/normalized features when needed

---

## Exploratory Data Analysis (EDA)
- Visualized feature distributions using histograms and bar plots
- Examined relationships between features and the target variable
- Checked correlations using heatmaps

---

## Feature Selection
- Calculated Variance Inflation Factor (VIF) for numerical features
- Selected features with VIF < 5 to avoid multicollinearity

---

## Model Building
- **Logistic Regression** – baseline model
- **Decision Tree Classifier** – with and without hyperparameter tuning
- **Random Forest Classifier** – final model with best accuracy
- Hyperparameter tuning using GridSearchCV for Decision Tree

---

## Results

| Model                     | Accuracy |
|----------------------------|---------|
| Logistic Regression        | 61.07%  |
| Decision Tree              | 65.06%  |
| Decision Tree (GridSearch) | 67.68%  |
| Random Forest              | 76.91%  |

- Random Forest achieved the **best performance**.

---

## Conclusion
- Random Forest performed best for credit score prediction.
- Feature selection and preprocessing improved model performance.
- Dataset cleaning, handling missing values, and outlier removal were crucial steps.

---

## Future Work
- Experiment with other ensemble methods like **XGBoost or LightGBM**
- Feature engineering for more predictive power
- Deploy model using Flask/Django or Power BI dashboards
- Integrate more external data for better predictions

---

## Technologies Used
- Python 3.x
- Pandas, NumPy, Matplotlib, Seaborn
- Scikit-learn (ML models)
- Google Colab (notebook environment)
