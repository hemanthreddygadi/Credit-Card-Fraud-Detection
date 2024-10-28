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
The dataset used for this project is sourced from [Kaggle](https://www.kaggle.com/dalpozz/creditcard-fraud) and contains transactions made by credit cards in September 2013 by European cardholders. It includes:
- 284,807 transactions labeled as either legitimate (`Class = 0`) or fraudulent (`Class = 1`).
- Features generated through PCA (Principal Component Analysis) to protect sensitive information.

## Setup
To set up the project locally, ensure you have Python installed. Then, clone this repository and install the required libraries using pip:

```bash
git clone https://github.com/yourusername/credit-card-fraud-detection.git
cd credit-card-fraud-detection
pip install -r requirements.txt
