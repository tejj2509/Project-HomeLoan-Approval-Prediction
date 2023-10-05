# Project-HomeLoan-Approval-Prediction
This is an End to End project on how to build a Machine Learning model that helps to predict if the applicant is eligible to be approved of a loan by a financial institution.

Loan approval prediction, aims at predicting if the customer is eligible to be sanctioned a loan based on some critical input features that the loan repayment ability relies on. Using this model, the financial institution can check the eligibility of the customer applying for loans. This can be used as an initial examination to evaluate if the customer will be promising with respect to the debt repayment and once there is an estimation that the person is eligible, the mortgage underwriters can then use the detailed analysis such as Credit, Capacity, Capital and Collateral evaluation methods based on the respective guidelines and come to a more precise conclusion if the loan can be sanctioned to the customer or not with very low risks for the funding financial institutions.

About Dataset

This data set contains details of a loan applicant, and the target variable showing if the customer will be approved with a loan.

Link: https://www.kaggle.com/datasets/rishikeshkonapure/home-loan-approval


Features Are as follows:


Loan_ID:

Unique Loan ID.


Gender:

If the applicant is Male/ Female.


Married:

Marital status of the applicant.


Dependents:

Number of dependents of the applicant.


Education	:

Applicant Education Qualification (Graduate/ Under Graduate).


Self_Employed:

Self-employed (Y/N).


ApplicantIncome:

Applicant's income in Dollars.


CoapplicantIncome:

Co-applicant's(If any) income in Dollars.


LoanAmount:

Loan amount	in Thousand Dollars.


Loan_Amount_Term:

Term of the loan in months.


Credit_History:

credit history meets guidelines(1 if yes and 0 if no).


Property_Area:

Property is located in Urban/ Semi Urban/ Rural.


Loan_Status:

Yes if the loan is approved and No if the loan is declined.


The dataset can also be found within this repository.

Data Preprocessing is done by using label encoding, one hot encoding, imbalance data treatment by using Over Sampling technique.

Exploratory Data Analysis (EDA) has been performed to understand the distribution and behaviour of all the input features.

Model Building Logistic Regression for binary classification, Random Forest, Bagging Classifier models are used and to build the final implementable machine learning model Bagging Classifier model is used. The model is having train and test accuracy of 83% and 75% repectively on 10 Cross Validation folds.

Model Evaluation: Model's performance has been evaluated using Classification Report, Confusion Matrix, Accuracy score and Cross Validation tests for both test and train datasets.

Usage: The model can be trained as shown in the .ipynb file and relevant input variables can be given to predict the output by using the following example code: prediction = bgc.predict([[Married, Education, ApplicantIncome, CoapplicantIncome, LoanAmount, Credit_History, Property_Area_Semiurban, Property_Area_Urban]])

Outcome: 'The applicant can be approved a loan for the said loan amount 118.0 Thousand Dollars.'
