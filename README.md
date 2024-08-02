## Challenge 21
## Project Title: Predicting Loan Status Using Machine Learning

## Introduction
This project aims to predict whether loans are healthy (0) or high-risk (1) using machine learning. The dataset includes financial and demographic details about borrowers and their loan applications. The goal is to create a model that accurately predicts loan status, helping financial institutions reduce risk and make better lending decisions.

## Installation
For this project, I needed to install the following:
* pip install tensorflow

## Dataset
* EIN: Employer Identification Number (removed during preprocessing)
* NAME: Name of the organization (removed during preprocessing)
* Additional demographic and financial features.
* APPLICATION_TYPE: Type of loan application
* CLASSIFICATION: Classification of the borrower
* ASK_AMT: Amount requested in the loan application
* IS_SUCCESSFUL: Target variable indicating loan status (1 for successful/healthy, 0 for unsuccessful/high-risk)

## Important Preprocessing Steps (hints)

* Data Preprocessing Steps:
Dropped Non-Beneficial Columns:
Removed columns that do not contribute to the prediction model.
* Value Count Analysis:
For columns with more than 10 unique values (APPLICATION_TYPE and CLASSIFICATION), determined the number of data points for each unique value.
* Binning Rare Categorical Values:
Chose cutoff points (600 for APPLICATION_TYPE and 300 for CLASSIFICATION) to group rare categorical values into a new value called "Other".
* Categorical to Numeric Conversion:
Used pd.get_dummies() to convert categorical data to numeric.
* Data Splitting:
Divided the data into a target array (IS_SUCCESSFUL) and features arrays.
* Train-Test Split:
Applied train_test_split to create testing and training datasets.
* Data Scaling:
Used StandardScaler to scale the training and testing sets.


## References
IRS. Tax Exempt Organization Search Bulk Data Downloads. https://www.irs.gov/Links to an external site.

