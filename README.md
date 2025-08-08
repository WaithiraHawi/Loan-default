# Loan Default Risk Analysis & Customer Segmentation

## Project Overview

This project analyzes a **Loan Default dataset** to explore patterns and factors influencing loan default risk.
In addition, it applies **customer segmentation** techniques to group borrowers into meaningful clusters and builds **default risk profiles** for each segment.
The goal is to provide **actionable insights** for credit risk teams and financial institutions to optimize lending decisions.

<img width="1024" height="1024" alt="Loan default" src="https://github.com/user-attachments/assets/b12b0d2d-c1e6-4b62-a3a6-ab9fed6a9a4e" />

## Dataset

* **File:** `Loan_default.csv`
* **Description:** Contains customer demographic details, loan attributes, and default status.
* **Key Features:**

  * `Customer_ID` – Unique customer identifier
  * `Age` – Age of the borrower
  * `Income` – Monthly/annual income
  * `LoanAmount` – Loan amount approved
  * `Loan_Term` – Duration of the loan
  * `Credit_Score` – Credit score of the customer
  * `Default` – Target variable (1 = default, 0 = no default)
  * Other possible features: Employment type, marital status, purpose of loan, etc.

## Technologies Used

* **Python** (Data Analysis & Machine Learning)
* **Pandas** – Data manipulation
* **NumPy** – Numerical operations
* **Matplotlib** / **Seaborn** – Data visualization
* **Scikit-learn** – Machine learning & clustering
* **Jupyter Notebook** – Analysis environment


## Analysis Workflow

### 1️Data Preprocessing

* Load dataset and inspect structure
* Handle missing values
* Encode categorical variables
* Remove outliers if necessary
* Standardize numerical features for clustering

### Exploratory Data Analysis (EDA)

* Univariate analysis (distribution plots)
* Bivariate analysis (correlation heatmaps, scatter plots)
* Default rate analysis by demographic & loan features
* Feature importance using **Random Forest Classifier**

### Default Risk Profiling

* Identify top predictors of default
* Build profiles for **High**, **Medium**, and **Low** risk borrowers
* Calculate default probability per profile

### Customer Segmentation (K-Means Clustering)

* Normalize features
* Determine optimal number of clusters (Elbow Method & Silhouette Score)
* Apply K-Means clustering
* Visualize customer segments
* Link clusters with default risk to create actionable strategies

## Key Insights 

* Customers with **low credit scores** and **high loan amounts** have the highest default probability
* Younger borrowers tend to have slightly higher risk levels compared to older borrowers
* Three customer segments were identified:

  * **Cluster 1:** High-income, low-risk borrowers
  * **Cluster 2:** Medium-income, moderate-risk borrowers
  * **Cluster 3:** Low-income, high-risk borrowers

## Next Steps

* Incorporate advanced ML models (XGBoost, LightGBM) for better prediction
* Develop an interactive dashboard for risk visualization
* Integrate the model into a loan approval API
