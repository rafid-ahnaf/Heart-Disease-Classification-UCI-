# Heart-Disease-Classification-UCI

## *Notebook Documentation:*

## **1. Introduction:**

This repository provides a comprehensive overview of the steps taken to analyze and model a medical Heart Disease dataset using various machine learning techniques. The primary goal was to predict the health condition of individuals based on a set of features. 

Dataset Description:

Dataset Name: Heart Disease UCI

Source: UCI Machine Learning Repository

Link: Heart Disease

https://archive.ics.uci.edu/dataset/45/heart+disease


## **2. Data Loading and Preprocessing:**

1. The dataset was loaded from a `.mod` file and parsed into a Pandas DataFrame.
2. Missing values were handled by replacing '?' with NaN and dropping rows with missing values in specific columns.
3. The redundant 'target' column was dropped as it contained the same information as the 'health' column.
4. Label encoding was used to transform categorical features into numerical values.
5. MinMaxScaler was employed to scale all numerical features between 0 and 1.

## **3. Data Exploration and Analysis:**

1. The distribution of the 'health' target variable was analyzed to identify any imbalances.
2. SMOTE (Synthetic Minority Over-sampling Technique) was applied to the training data to address the imbalance by generating synthetic samples of the minority class.
3. Correlation analysis was performed to investigate the relationships between features and the target variable.

## **4. Model Training and Evaluation:**

1. Three machine learning models were trained on the balanced training data:
    - Logistic Regression
    - Random Forest
    - XGBoost
2. Each model was evaluated on the test data using various metrics such as accuracy, precision, recall, and F1 score.
3. Confusion matrices were visualized for each model to gain insights into their performance.

## **5. Conclusion:**

Based on the evaluation results, the XGBoost model demonstrated the best performance in predicting the health condition of individuals. However, further optimization and analysis could be conducted to refine the model and improve its accuracy.

## **Additional Notes:**

- The code provided in this notebook can be readily executed and modified to explore different aspects of the data and experiment with alternative modeling techniques.
- The documentation serves as a valuable reference for understanding the steps taken and the rationale behind each decision made during the analysis process.
