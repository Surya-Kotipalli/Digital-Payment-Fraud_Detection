# Dataset

## Dataset Overview

This project uses a real-world digital payment transaction dataset for fraud detection analysis and machine learning classification.

### Dataset Size

- Total Records: **1,048,575 transactions**
- Fraudulent Transactions: **1,142**
- Normal Transactions: **1,047,433**
- Fraud Ratio: **~0.1% of total data**

The dataset is highly imbalanced, making fraud detection a challenging classification problem.

---

## Dataset Attributes

| Attribute | Description |
|---|---|
| `step` | Time step of the transaction |
| `type` | Type of transaction (PAYMENT, TRANSFER, CASH_OUT, DEBIT, CASH_IN) |
| `amount` | Amount involved in the transaction |
| `oldbalanceOrg` | Sender's account balance before transaction |
| `newbalanceOrig` | Sender's account balance after transaction |
| `oldbalanceDest` | Receiver's account balance before transaction |
| `newbalanceDest` | Receiver's account balance after transaction |
| `isFraud` | Target variable indicating fraudulent transaction (0 = Normal, 1 = Fraud) |
| `isFlaggedFraud` | System-generated fraud flag for suspicious high-value transfers |

---

## Dataset Characteristics

- Large-scale financial transaction dataset
- Highly imbalanced fraud distribution
- Includes both categorical and numerical attributes
- Contains transaction behavior and balance information
- Suitable for classification, anomaly detection, and fraud analytics tasks

---

## Key Observations

Fraudulent transactions were predominantly observed in:
- `TRANSFER`
- `CASH_OUT`

Transaction types such as:
- `PAYMENT`
- `CASH_IN`
- `DEBIT`

showed minimal or no fraudulent activity in the dataset.

---

## Purpose

The dataset was used to:
- Perform exploratory data analysis (EDA)
- Engineer fraud-related behavioral features
- Train and evaluate machine learning classification models
- Analyze fraud patterns and transaction anomalies
- Compare predictive model performance using Recall, Precision, and F1-score
