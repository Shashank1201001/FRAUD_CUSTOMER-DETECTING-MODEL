Fraudulent Transaction Prediction Project

Project Overview:
The main objective of this data science project is to develop a machine learning model to predict fraudulent transactions for a financial company. The goal is to detect and prevent fraudulent activities, thereby safeguarding the company and its customers from potential financial losses and reputational damage.

Dataset Description:
The dataset used in this project maps a unit of time in the real world, where 1 step represents 1 hour of time. The total number of steps is 744, equivalent to a 30-day simulation. The dataset includes the following columns:
type: The type of transaction, which can be one of the following: CASH-IN, CASH-OUT, DEBIT, PAYMENT, or TRANSFER.
amount: The amount of the transaction in the local currency.
nameOrig: The customer who initiated the transaction.
oldbalanceOrg: The initial balance of the customer's account before the transaction.
newbalanceOrig: The new balance of the customer's account after the transaction.
nameDest: The recipient of the transaction. Note that there is no information provided for customers whose names start with 'M' (Merchants).
oldbalanceDest: The initial balance of the recipient's account before the transaction. Note that there is no information provided for customers whose names start with 'M' (Merchants).
newbalanceDest: The new balance of the recipient's account after the transaction. Note that there is no information provided for customers whose names start with 'M' (Merchants).
isFraud: Indicates transactions made by fraudulent agents within the simulation. The fraudulent behavior of these agents aims to take control of customers' accounts and attempt to empty the funds by transferring to another account and then cashing out of the system.
isFlaggedFraud: The business model aims to control massive transfers from one account to another and flags illegal attempts. An illegal attempt in this dataset is an attempt to transfer more than $200,000 in a single transaction.

Approach and Model Evaluation:
To predict fraudulent transactions, various machine learning models were evaluated. After thorough experimentation, the Gradient Boosting model emerged as the best-performing choice. Here are the key points regarding the approach and model evaluation:
Model Selection: Gradient Boosting was selected due to its high accuracy and recall.
Accuracy: The model achieved an accuracy of 98%.
Recall: The model demonstrated a good recall of 98% for both fraudulent and non-fraudulent classes.

To address class imbalance in the dataset, the Synthetic Minority Over-sampling Technique (SMOTE) was employed. SMOTE generates synthetic samples of the minority class, balancing the dataset and allowing the model to learn from a more representative distribution of fraudulent transactions.

Conclusion:
The developed model for predicting fraudulent transactions in the financial domain achieved remarkable accuracy and recall rates. By utilizing Gradient Boosting and applying SMOTE to address class imbalance, the project effectively mitigated the risks associated with fraud.

This model can be integrated into the financial company's system to proactively identify and prevent fraudulent activities, safeguarding the company's assets and maintaining the trust of its customers.
