# 💳 Credit Score Classification  

This project aims to classify individuals’ **credit scores** based on financial and behavioral features using machine learning algorithms such as **Logistic Regression**, **Decision Tree**, and **Random Forest**.  

---

## 📑 Table of Contents  
1. [Overview](#overview)  
2. [Dataset Information](#dataset-information)  
3. [Data Preprocessing](#data-preprocessing)  
4. [Plots & Visualizations](#plots--visualizations)  
5. [Model Building](#model-building)  
6. [Model Comparison](#model-comparison)  
7. [Results](#results)  
8. [Jupyter Notebook / Google Colab](#-jupyter-notebook--google-colab)  
9. [Conclusion](#conclusion)  

---

## 🧩 Overview  
The goal of this project is to predict a customer’s **credit score** (Good, Standard, Poor) based on key financial metrics and credit behaviors.  
This helps financial institutions in making better lending and risk-assessment decisions.  

---

## 📊 Dataset Information  

| Column | Description |
|:--|:--|
| Age | Age of the customer |
| Occupation | Type of occupation |
| Annual Income | Annual income of the customer |
| Monthly Inhand Salary | Monthly in-hand salary |
| Num Bank Accounts | Number of bank accounts |
| Num Credit Card | Number of credit cards |
| Interest Rate | Rate of interest on loans |
| Num of Loan | Total number of loans |
| Delay from due date | Average days delayed for payment |
| Num of Delayed Payment | Number of delayed payments |
| Credit Mix | Type of credit behavior (Good / Standard / Bad) |
| Outstanding Debt | Total outstanding debt |
| Credit Utilization Ratio | Percentage of credit used |
| Payment of Min Amount | Whether minimum amount is paid |
| Total EMI per month | Total EMI amount paid per month |
| Amount invested monthly | Investment amount per month |
| Payment Behaviour | Customer’s payment habits |
| Monthly Balance | Monthly balance left after expenses |
| Credit Score | Target variable (Good / Standard / Poor) |

---

## 🧹 Data Preprocessing  

- Removed or replaced **special characters**.  
- Converted all applicable columns to **int/float** datatypes.  
- Handled **missing values** using forward and backward filling.  
- Applied **Label Encoding** to categorical columns.  
- Standardized numerical features before model training.  

---

## 📈 Plots & Visualizations  

### Distribution Analysis  
![Months](images/plots/Distribution%20of%20months.png)  
![Payment of Min Amount](images/plots/Distribution%20of%20Payment_of_Min_Amount.png)  
![Payment Behaviour](images/plots/Distribution%20of%20Payment%20Behaviour.png)  
![Occupation](images/plots/Distribution%20of%20Occupation.png)  
![Credit Mix](images/plots/Distribution%20of%20Credit%20Mix.png)  
![Credit Score Distribution](images/plots/Credit%20Score%20Distribution.png)  

### Age Analysis  
![Age Outliers](images/plots/df['Age']%20Outliers.png)  
![Age Boxplot](images/plots/Age%20Boxplot.png)  

### Model Comparison  
![ML Models Comparison](images/plots/Comparision%20of%20ML%20Models.png)  

---

## 🤖 Model Building  

Three machine-learning models were trained and evaluated:  

- **Logistic Regression (LR)**  
- **Decision Tree (DT)**  
- **Random Forest Classifier (RFC)**  

Hyperparameter tuning was done using **GridSearchCV** for Decision Tree.  

---

## ⚖️ Model Comparison  

| Model | Accuracy |
|:--|:--:|
| Logistic Regression | ~61% |
| Decision Tree | ~65% |
| Decision Tree with Hyper Parameter | ~67% |
| Random Forest | ~77% |

---

## 📓 Jupyter Notebook / Google Colab  

You can open and explore the full notebook directly in Google Colab using the link below 👇  

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Pushpendra54-DS/Credit_Score_Classification/blob/main/notebooks/Credit_score.ipynb)

---

## 🏁 Conclusion  

- Random Forest outperformed other models in accuracy.  
- Proper data cleaning and encoding significantly improved model performance.  
- Feature importance analysis shows that **Payment Behaviour**, **Credit Mix**, and **Outstanding Debt** have the strongest impact on credit score prediction.  

---

✅ **Author:** Pushpendra Singh  
📘 **Repository:** [Credit_Score_Classification](https://github.com/Pushpendra54-DS/Credit_Score_Classification)

