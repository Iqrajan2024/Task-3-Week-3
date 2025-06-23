# Task 3: Customer Churn Prediction for Bank Customers

##  Overview
This project focuses on predicting **customer churn** — whether a bank customer will leave the bank — using supervised machine learning techniques. The analysis is based on the **Churn Modelling** dataset and includes data cleaning, exploratory analysis, model building, evaluation, and interpretation.

##  Objective
- Understand factors that lead to customer churn.
- Preprocess and prepare the data for machine learning.
- Train a classification model (Random Forest) to predict churn.
- Evaluate model performance and analyze feature importance.

##  Dataset Description
- **Target Variable:** `Exited` (1 = Customer left, 0 = Customer stayed)
- **Numerical Features:** Age, Balance, Credit Score, Tenure, Estimated Salary, etc.
- **Categorical Features:** Geography, Gender, HasCrCard, IsActiveMember, etc.
- **Imbalance:** 20% churners vs 80% non-churners

##  Data Preprocessing
- No missing or duplicate values found.
- Categorical variables encoded using **One-Hot Encoding**.
- Numerical features scaled appropriately.
- Addressed class imbalance using **oversampling**.

## Exploratory Data Analysis (EDA)

### ➤ Univariate & Bivariate Analysis
- Histograms, boxplots, and countplots were used.
- Churn rate is higher among older customers and those with lower account activity.
- Geography and credit card ownership slightly influence churn.

### ➤ Multivariate Analysis
- Correlation heatmaps and bar plots used to visualize feature relationships.

## Model Building

### Model Used: **Random Forest Classifier**
- Chosen for its robustness and ability to handle mixed feature types.

### Training and Testing
- Dataset split into training and testing sets (commonly 80/20).
- Model trained on oversampled data to address imbalance.

##  Evaluation Metrics
- **Accuracy** Model achieved 82% accuracy.
- **Precision, Recall, F1-score** (via classification report)
- **Confusion Matrix**

###  Performance:
- Model shows good accuracy and improved recall for minority class due to oversampling.

##  Key Insights
1. **Age** is the most influential factor — older customers are more likely to churn.
2. **Balance**, **EstimatedSalary**, and **CreditScore** are also strong indicators.
3. **Geography** and **Gender** have minimal influence on churn in this dataset.

## Technologies Used
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Jupyter Notebook

## Skills
- Categorical data encoding (Label Encoding / One-Hot Encoding)
- Supervised classification modeling
- Understanding and interpreting feature importance
