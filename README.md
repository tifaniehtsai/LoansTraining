# Loans Training
This project focuses heavily on cleaning the dataset, performing exploratory data analysis, and training and testing the data to see how many people repaid their loans.

## Dataset
Dataset: consists of LoansTrainingSet.csv, containing information about loaner properties. 
Features: Loan status, Loan ID, Customer ID, Current Loan Amount, and other attributes. 
Goal: clean the data in order to find the higher causes of loan defaulting

## Techniques
- EDA to understand the distribution of features and relationship with the target variable
- Visualizations such as histograms, heatmaps, and scatter plots

## In Depth Approach
1) Data Processing:
    - focused on removing duplicated Loan IDs first, did some EDA such as plotting a scatterplot of GrLivArea (ground living area square feet, chose this feature because highest numerical correlation to target) against SalePrice (target)
    - dropped unnecessary columns such as Utilities
    - checked for unusual values in Credit Score
    - impute nulls for Credit Score, Current Loan Amount, Years in Current Job, Annual Income as well as other features
    - transformed numerical features using Log1p and scaled using RobustScaler
    - encoded categorical features
2) Training Data
    - Used Smote, Undersample, and Oversampler to balance data


## Dependencies
- Python
- Libraries: pandas, numpy, matplotlib, seaborn, scikit-learn
