## 📊 Loan Approval Prediction
  A machine learning project to predict whether a loan application will be approved based on various applicant and loan-related features.
  
  ## 📌 Objective
The goal of this project is to **analyze patterns** in customer and loan data and build a predictive model to determine the likelihood of loan approval (`loan_status`).

## 🧩 Dataset Overview

|Feature | Description|
|----------|----------|
|`person_age`|Age of the applicant
`person_income`|Applicant's income
`person_emp_exp`|Years of employment experience
`loan_amnt`|Amount of loan requested
`loan_int_rate`|Interest rate of the loan
`loan_percent_income`|Loan amount as a % of income
`credit_score`|Applicant's credit score
`loan_status`|Target variable (1 = approved, 0 = not)

The dataset was cleaned and preprocessed to remove outliers, impute missing values, and convert categorical variables using One-Hot Encoding.

## 🛠️ Tools and Libraries

-   `pandas`, `numpy` – Data manipulation
    
-   `seaborn`, `matplotlib` – Data visualization, Exploration Data
    
-   `scikit-learn` – Model building, pipeline, and evaluation
    
-   `Pipeline + ColumnTransformer` – For clean preprocessing
    
-   `RandomForestClassifier`, `DecisionTreeClassifier`, `KMeans`

## 📈 Model Evaluation

-   Used `Accuracy`, `Precision` to evaluate models
    
-   Applied `Cross-Validation` to avoid overfitting
    
-   Tuned hyperparameters such as `n_estimators` in Random Forest
    

> **Best Accuracy:** 91.45% with RandomForest (n_estimators = 50)

![image](https://github.com/user-attachments/assets/84d4ec01-d9bc-4acc-8aaa-49babc1d6beb)

![image](https://github.com/user-attachments/assets/9b28c5a1-50fb-4fd5-933a-f8dbac93b058)

## 🔍 Feature Importance

Top contributing features value top 5 importance :

-   `person_income` 
    
-   `loan_int_rate`
    
-   `loan_percent_income` 
    
-   `previous_loan_defaults_on_file` :  Value is "No" 

-   `previous_loan_defaults_on_file` : Value is "Yes"

![image](https://github.com/user-attachments/assets/d4b05236-e7ba-44e6-a26b-a68e51a0bc19)

## 🚀 How to Run

1.  Clone the repository
    
2.  Install requirements: `pip install -r requirements.txt`
    
3.  Run the notebook: `loan_approval_prediction.ipynb`

## 💡 Conclusion

This project demonstrates how data science and machine learning can be used to support **financial decision-making**, reduce risk, and speed up **loan approval processes**. The use of feature importance and visualization helps stakeholders understand what factors affect decisions the most.
