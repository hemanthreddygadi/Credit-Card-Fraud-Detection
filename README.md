# Credit-Card-Fraud-Detection
# Credit Card Fraud Detection

## Overview
This project focuses on detecting fraudulent transactions in credit card data using machine learning techniques. The dataset consists of various transactions, classified as legitimate or fraudulent. We employ logistic regression to build a predictive model, evaluate its performance, and interpret the results.

## Table of Contents
- [Technologies Used](#technologies-used)
- [Dataset](#dataset)
- [Setup](#setup)
- [Usage](#usage)
- [Model Evaluation](#model-evaluation)
- [Results](#results)
- [License](#license)

## Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

## Dataset
The dataset used for this project is sourced from [Kaggle](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud) and contains transactions made by credit cards in September 2013 by European cardholders. It includes:
- 284,807 transactions labeled as either legitimate (`Class = 0`) or fraudulent (`Class = 1`).
- Features generated through PCA (Principal Component Analysis) to protect sensitive information.

## Setup
To set up the project locally, ensure you have Python installed. Then, clone this repository and install the required libraries using pip:

1. **Install Python**: Ensure you have Python installed on your system. You can download it from [python.org](https://www.python.org/downloads/).

2. **Install Jupyter Notebook**: If you don't have Jupyter Notebook installed, you can install it using pip. Open your terminal or command prompt and run:
   ```bash
   pip install notebook

## Usage
Load the dataset using Pandas.
Preprocess the data.
Handle missing values.
Scale the features.
Split the dataset into training and testing sets.
Train the logistic regression model on the training set.
Evaluate the model's performance on the test set.

## Modal Evalaution
## Model Evaluation

### 1. Accuracy

Accuracy measures the proportion of true results among the total number of cases examined. It is calculated using the formula:

\[ \text{Accuracy} = \frac{\text{TP} + \text{TN}}{\text{TP} + \text{TN} + \text{FP} + \text{FN}} \]

Where:
- **TP** = True Positives (correctly predicted positive cases)
- **TN** = True Negatives (correctly predicted negative cases)
- **FP** = False Positives (incorrectly predicted positive cases)
- **FN** = False Negatives (incorrectly predicted negative cases)

High accuracy indicates that the model performs well overall, but it may not provide a complete picture, especially in imbalanced datasets.

### 2. Confusion Matrix

The confusion matrix is a table that summarizes the performance of a classification model. It provides a detailed breakdown of correct and incorrect predictions, allowing for a clearer understanding of the model's strengths and weaknesses.

A typical confusion matrix looks like this:

          Predicted
           0     1
        0  TN    FP

- **True Positives (TP)**: Correctly predicted fraudulent transactions.
- **True Negatives (TN)**: Correctly predicted legitimate transactions.
- **False Positives (FP)**: Legitimate transactions incorrectly classified as fraudulent.
- **False Negatives (FN)**: Fraudulent transactions incorrectly classified as legitimate.

### 3. Learning Curve

Learning curves provide insights into how the model's performance changes as the amount of training data increases. They plot the training and validation scores against the number of training instances.

Key interpretations of learning curves include:
- **Underfitting**: Both training and validation scores are low, indicating that the model is too simple.
- **Overfitting**: Training score is high while validation score is low, indicating that the model is too complex and fails to generalize.
- **Appropriate Fit**: Both scores converge at a high value, indicating a well-fit model.

Learning curves help identify whether more data could improve model performance.

### 4. Feature Importance

Feature importance assesses the contribution of each feature to the model's predictions. In logistic regression, the coefficients of the features indicate their importance, with larger absolute values reflecting greater influence on the target variable.

By analyzing feature importance, we can:
- Identify which features contribute most to the model's predictions.
- Inform feature selection for improving model performance.
- Enhance model interpretability.

Visualizing feature importance (e.g., with a bar chart) can provide a clear overview of which features are most critical in the model's decision-making process.

---

These metrics collectively provide a comprehensive understanding of the model's performance and guide further improvements.

```bash
git clone https://github.com/hemanthreddygadi/Credit-Card-Fraud-Detection
cd credit-card-fraud-detection
pip install -r requirements.txt
