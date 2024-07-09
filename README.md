CODETECH Task 1

Name - Sadhav Singh
Comapny - CODTECH IT SOLUTIONS
ID - CT6WDS79
Domain - MACHINE LEARNING
Duration - 1st JUNE 2024 to 13Th JULY 2024
Mentor - G.SRAVANI

Overview of Project

1. Objective
    The primary goal of this project is to build and deploy a logistic regression model to detect fraudulent credit card transactions.

2. Dataset
    The dataset creditcard.csv contains credit card transactions, where:
    Each row represents a transaction.
    The column Class indicates whether the transaction is legitimate (0) or fraudulent (1).
    Other columns represent various features of the transactions.
   
4. Data Preparation
    Loading Data: The dataset is loaded into a Pandas DataFrame.
    Separating Transactions:
    Legitimate transactions are separated into legit.
    Fraudulent transactions are separated into fraud.
    Balancing Classes:
    Legitimate transactions are undersampled to match the number of fraudulent transactions to address class imbalance.
    The balanced dataset is created by concatenating the undersampled legitimate transactions and fraudulent transactions.

6. Model Training
    Feature and Target Separation:
    Features (X) are all columns except Class.
    Target (y) is the Class column.
    Train-Test Split:
    The dataset is split into training and testing sets with an 80-20 ratio, maintaining class distribution (stratify=y).
    Training the Model:
    A Logistic Regression model is instantiated and trained on the training set.

8. Model Evaluation
    Accuracy Calculation:
    Training accuracy is calculated using predictions on the training set.
    Testing accuracy is calculated using predictions on the testing set.

10. Deployment Using Streamlit
Streamlit Application:
Title and author information are displayed.
A text input field is provided for the user to enter feature values.
A button allows the user to submit these values.

Prediction:
    Upon clicking the submit button, the feature values are read, and the model makes a prediction.
    The prediction result is displayed as either "Legitimate transaction" or "Fraudulent transaction".
