**Credit Card Fraud Detection**

**About the Dataset:**
This project utilizes a simulated credit card transaction dataset that contains both legitimate and fraudulent transactions recorded from January 1, 2019, to December 31, 2020. The dataset includes transactions made by 1000 customers at 800 different merchants.
Data Description:
fraudTrain.csv: Training dataset with fraudulent and non-fraudulent transactions.
fraudTest.csv: Testing dataset with fraudulent and non-fraudulent transactions.
You can access the dataset on Kaggle via this link: https://www.kaggle.com/datasets/kartik2112/fraud-detection

**Project Overview:**
This project aims to detect fraudulent credit card transactions using various machine learning classifiers. The following steps are undertaken:

**Data Loading and Preprocessing:**
The data loading and preprocessing steps involve reading the CSV files into pandas DataFrames and performing initial cleaning and transformation of the data.

Loading the Data:
The dataset is loaded into data structures suitable for analysis. The project utilizes a sample of 100,000 records from the training data and 50,000 records from the testing data to ensure efficient processing.

Inspecting the Data:
Basic information about the data is examined to understand its structure, including checking for data types, missing values, and summary statistics.

Dropping Unnecessary Columns:
Irrelevant columns such as identifiers and personal information are removed to streamline the dataset and focus on features that are relevant to detecting fraud.

Handling Date and Time Data:
Transaction date and time are converted to appropriate formats, and additional features such as the cardholder's age at the time of transaction are calculated. This helps in extracting meaningful insights and patterns from the data.

**Exploratory Data Analysis (EDA):**
EDA involves visualizing and understanding the patterns and distributions in the data.

Histograms and Box Plots:
Visualizations are used to explore the distribution of numerical features. Histograms help in understanding the frequency distribution, while box plots are useful for identifying outliers and the spread of the data.

Pie Chart for Fraud Distribution:
The proportion of fraudulent versus non-fraudulent transactions is visualized using pie charts, providing a clear picture of the class imbalance in the dataset.

**Feature Engineering:**
Feature engineering involves transforming raw data into features that better represent the underlying problem to the predictive models.

Encoding Categorical Features:
Categorical features such as merchant names, transaction categories, and customer information are encoded into numerical values. This step is crucial for machine learning models to process categorical data effectively.

Standardizing Numerical Features:
Numerical features are standardized to ensure they have zero mean and unit variance. Standardization improves the performance of many machine learning models by ensuring that features are on a similar scale.

Extracting Date and Time Features:
Additional features are extracted from the transaction timestamp, including the year, month, day, hour, minute, and second of the transaction. These features can capture temporal patterns that may be indicative of fraud.

**Model Training and Evaluation:**
The following machine learning models were trained and evaluated:

1. Support Vector Machine (SVM)
2. Random Forest
3. LightGBM
4. XGBoost

**Model Comparison:**
Evaluation Metrics
Accuracy
Precision
Recall
F1 Score
Confusion matrices were also plotted to visualize the performance of each model.

**Dependencies:**
Make sure you have the following dependencies installed:
pandas

scikit-learn

category_encoders

nump

matplotlib

seaborn

xgboost

lightgbm

catboost
