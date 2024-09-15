# Credit Card Fraud Detection

## Project Overview
A credit card is one of the most used financial products to make online purchases and payments. Though the Credit cards can be a convenient way to manage your finances, they can also be risky. Credit card fraud is the unauthorized use of someone else's credit card or credit card information to make purchases or withdraw cash.

It is important that credit card companies are able to recognize fraudulent credit card transactions so that customers are not charged for items that they did not purchase.

The dataset contains transactions made by credit cards in September 2013 by European cardholders. This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.

We have to build a classification model to predict whether a transaction is fraudulent or not.

## Dataset Description
The dataset consists of 31 columns and 284,807 rows. Each row represents a single transaction. The attributes in the dataset are as follows:

### Attributes
1. **Time**: The number of seconds elapsed between this transaction and the first transaction in the dataset.
2. **V1, V2, ..., V28**: These are the principal components obtained using PCA (Principal Component Analysis). Due to confidentiality issues, the original features are not provided, and only the transformed features are available.
3. **Amount**: The transaction amount. This feature can be used for example-dependent cost-sensitivity analysis.
4. **Class**: The response variable and it takes the value 1 in case of fraud and 0 otherwise.

### Data Distribution
- **Non-fraudulent transactions**: 284,315
- **Fraudulent transactions**: 492

### Data Imbalance
The dataset is highly imbalanced, with fraudulent transactions accounting for only 0.172% of all transactions. Special techniques such as resampling, SMOTE (Synthetic Minority Over-sampling Technique), or anomaly detection methods may be required to handle this imbalance.

## Data Preprocessing
1. **Handling Missing Values**: There are no missing values in the dataset.
2. **Scaling**: The `Amount` and `Time` features are scaled using standard scaling techniques.
3. **Dimensionality Reduction**: PCA has already been applied to the original features, resulting in the `V1` to `V28` attributes.

## Model Building
Several machine learning models are trained and evaluated, including:
- Logistic Regression
- Decision Trees
- Random Forest


## Evaluation Metrics
Given the imbalanced nature of the dataset, the following metrics are used to evaluate model performance:
- accuracy score

## Instructions to Run the Project
1. Clone the repository:
   ```bash
   git clone https://github.com/a s vani/credit-card-fraud-detection.git

Navigate to the project directory:
cd credit-card-fraud-detection

Install the required dependencies:
pip install -r requirements.txt

Run the Jupyter notebooks or Python scripts in the notebooks folder to perform data exploration, preprocessing, and model building.
Conclusion
This project demonstrates the application of machine learning techniques to detect fraudulent credit card transactions. 

References
creditcard.csv
