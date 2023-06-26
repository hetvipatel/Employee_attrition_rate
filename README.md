# Employee Attrition Prediction

This repository contains a machine learning project that focuses on predicting employee attrition using various algorithms. The dataset used in this project is the IBM HR Analytics Attrition Dataset.

## Table of Contents
- [Introduction](#introduction)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)
  

## Introduction
Employee attrition, or employee turnover, is a critical concern for organizations. This project aims to predict employee attrition by analyzing various factors such as age, monthly income, and department. Different machine learning algorithms, including Logistic Regression, XGBoost, Decision Tree, and Random Forest, are implemented and evaluated to determine their predictive performance.

## Installation
To run the code and reproduce the results locally, follow these steps:
1. Clone this repository: `git clone <repository-url>`
2. Install the required libraries: `pip install pandas matplotlib seaborn sklearn xgboost`

## Usage
1. Load the dataset: The IBM HR Analytics Attrition Dataset is loaded using `pd.read_csv()` function. Update the file path in the code to the appropriate location on your machine.
2. Exploratory Data Analysis (EDA): EDA is performed to gain insights into the dataset. The `head()` and `info()` methods are used to display the first few rows and get information about the dataset, respectively.
3. Data Cleaning: Any missing values in the dataset are dropped using the `dropna()` method.
4. Data Visualization: Matplotlib and Seaborn libraries are used to visualize the data. Two examples are shown in the code: a countplot of attrition and a boxplot of monthly income distribution by department.
5. Data Preprocessing: The target variable 'Attrition' is mapped to binary values (1 for 'Yes' and 0 for 'No'). Selected features are extracted from the dataset and one-hot encoded using `get_dummies()` function.
6. Splitting the Dataset: The dataset is split into training and testing sets using the `train_test_split()` method from scikit-learn.
7. Implementing Machine Learning Algorithms: Logistic Regression, XGBoost, Decision Tree, and Random Forest classifiers are initialized and trained using the training data.
8. Model Evaluation: The accuracy score and confusion matrix are computed to evaluate the performance of each algorithm on the testing data.
9. Results: The results, including accuracy and confusion matrix, are printed for each algorithm.

## Results
The results of running the machine learning algorithms are as follows:
- Logistic Regression Accuracy: 0.8616780045351474
- Logistic Regression Confusion Matrix:
  ```
  [[380   0]
  [ 61   0]]
  ```
- XGBoost Classifier Accuracy: 0.9954648526077098
- XGBoost Classifier Confusion Matrix:
  ```
  [[380   0]
   [  2  59]]
  ```
- Decision Tree Accuracy: 0.7709750566893424
- Decision Tree Confusion Matrix:
  ```
  [[326  54]
  [ 47  14]]
  ```
- Random Forest Accuracy: 0.8253968253968254
- Random Forest Confusion Matrix:
  ```
  [[357  23]
  [ 54   7]]
  ```

## Contributing
Contributions to this project are welcome. Feel free to open issues or submit pull requests for any enhancements or bug fixes.
