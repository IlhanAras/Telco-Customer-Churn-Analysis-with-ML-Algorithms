# Telco-Customer-Churn-Analysis-with-ML-Algorithms
# The story of the datasets
Telco customer churn data, 7043 California home phone and Internet services provider fictitious in the third quarter.
Contains information about a telecom company. In which industries you have signed up for some or some of the services
shows.

# The data set includes information about:

Customers who left within the last month – the column is called Churn

Services that each customer has signed up for – phone, multiple lines, internet, online security, online backup, device protection, tech support, and streaming TV and movies

Customer account information – how long they’ve been a customer, contract, payment method, paperless billing, monthly charges, and total charges

Demographic info about customers – gender, age range, and if they have partners and dependents
# Stages of project
- Importing Dataset, Required Library and Functions
- Exploratory Data Analysis

    1. Overview
    2. Analysis of Categorical Variables
    3. Analysis of Numerical Variables
    4. Analysis of Target Variable
    5. Analysis of Correlation
-
- DATA PREPROCESSING

    1. Outliers (Aykırı Değerler)
    2. Missing Values (Eksik Değerler)
    3. Base Model
    4. Feature Extraction (Özellik Çıkarımı)
    5. Encoding (Label Encoding, One-Hot Encoding, Rare Encoding)
-
- Modelling

    1. Test Modelling
    2. Automated Hyperparameter Optimization
    3. Feature Importance
    4. Model Validation   
-
- Report
# Report
This project aims to develop a machine learning model that can predict the probability of customers leaving the company. Before the model is created, necessary data analysis and engineering steps will be taken.

## Stages conducted within the scope of the project:

### 1. Importing and Loading Phase:
- Required Libraries and Functions imported and dataset read

### 2. via Exploratory Data Analysis:
- The structural information of the data set was examined.
- Descriptive statistics of the data set were examined.
- The size information of the data set has been reached.
- The types of categorical and numerical variables in the data set were examined and visualized.
- Categorical and numerical variables were analyzed within themselves and by target variable.
- Correlation between variables observed and visualized.

### 3. In data preprocessing process:

- As a result of the outlier analysis, 0 variable with outliers were observed.
- As a result of missing value analysis, it was observed that 11 units were missing, approximately 0.16% of the observation units, in the variable "TotalCharges". These observation units were excluded from the project.
- During the feature exraction phase, 10 new variables were produced.
- Using One-Hot Encoding and Label Encoding techniques the data set was encoded to be ready for the use of machine learning algorithms.

### 4. In Model Building Phase:

- Firstly, with 7 classifier and regression techniques including LogisticRegression, KNeighborsClassifier, DecisionTreeClassifier,
RandomForestClassifier, SVC, XGBClassifier, LGBMClassifier machine learning algorithms, base models were established and "accuracy", "f1", "roc_auc", "precision", "recall" scores were observed.
- Then, in the Model Tuning and Evaluation phase, the best hyperparameters were reached by using the GridSearchCV technique.
- In the Feature Importance stage, the effects of each variable on the model was calculated and visualized, specific to various machine learning algorithms.

### 5. In Model Validation Phase:

- Model Complexity was analyzed using Learning Curves in terms of Random Forest and XGBOOST algorithms and their optimized parameters.

# Conclusion:

After all the analysis, data preprocessing, feature engineering, modeling and optimization stages on the data set, 

The Base Linear Regression (Base_LR) model stands out with high accuracy (0.802) and area under the curve (AUC) value (0.843). It also provides moderate recall (0.540) and precision (0.655). The F1 score is calculated as 0.592.

Base_KNN and Base_CART models exhibit lower recall and F1 score as base models. However, they can be preferred in cases where low computational cost is required.

Optimized models (Hyper_Param) generally outperform the base models. Especially, the LGBM_Hyper_Param model shines with high accuracy (0.803) and AUC (0.845) values.

In conclusion, we emphasize the importance of choosing a model depending on specific criteria or usage scenarios. Model selection should consider both the requirements of the workload and performance metrics.

This study lays a foundation for future research while indicating that further improvements, such as more hyperparameter tuning and feature engineering, could further enhance performance.
