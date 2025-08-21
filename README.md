Financial Fraud Detection Project
This repository contains a machine learning project to proactively detect fraudulent financial transactions. The solution was developed as part of a screening assignment and demonstrates a full data science workflow, from data analysis and feature engineering to model training and evaluation.

The primary goal is to build a robust model that accurately identifies fraudulent activities, helping a financial company minimize losses and protect its customers.

🚀 Project Overview
The project tackles the challenge of identifying fraudulent transactions within a large dataset. The core of the solution is a Random Forest Classifier, a powerful algorithm chosen for its high accuracy and its ability to handle the complex and imbalanced nature of fraud data.

Key Features:
Data Cleaning: The dataset was analyzed for inconsistencies and prepared for the modeling phase.

Feature Engineering: New, highly predictive features (errorBalanceOrig, errorBalanceDest) were engineered to capture transactional discrepancies that are strong indicators of fraud.

Model Training: A Random Forest Classifier was trained on the dataset, using a balanced class weight strategy to address the severe class imbalance between fraudulent and non-fraudulent transactions.

Performance: The final model demonstrates excellent performance, capable of identifying a high percentage of fraudulent transactions while keeping false positives to a minimum.

📊 Key Results & Findings
The model's performance was evaluated on a held-out test set, yielding strong results:

Precision (for Fraud class): 98% (When the model predicts a transaction is fraudulent, it is correct 98% of the time).

Recall (for Fraud class): 75% (The model successfully identifies 75% of all actual fraudulent transactions).

ROC AUC Score: 0.999 (Indicates outstanding capability to distinguish between classes).

Top 5 Predictors of Fraud:
The model identified the following features as the most important for detecting fraudulent activity:

errorBalanceOrig: The error in the originator's account balance after the transaction.

step: The specific time unit in the simulation, indicating temporal patterns.

type_PAYMENT: The type of transaction (used as a strong indicator of non-fraud).

amount: The monetary value of the transaction.

oldbalanceOrg: The initial balance of the sender's account.

🛠️ How to Run This Project
To replicate this analysis, please follow the steps below.

1. Prerequisites
You will need Python 3 installed, along with the following libraries:

pandas

scikit-learn

matplotlib

seaborn

2. Installation
You can install the required libraries using pip:

Bash

pip install pandas scikit-learn matplotlib seaborn
3. Execution
Clone this repository to your local machine:

Bash

git clone https://github.com/Aan9758/Your-Repository-Name.git
Place the Fraud3.csv dataset in the cloned repository's root directory.

Open and run the Jupyter Notebook (Fraud_Detection_Analysis.ipynb) to execute the code and view the full analysis.

💻 Technologies Used
Python 3

Pandas: For data manipulation and analysis.

Scikit-learn: For building and evaluating the machine learning model.

Matplotlib & Seaborn: For data visualization.

Jupyter Notebook: For interactive development and analysis.
