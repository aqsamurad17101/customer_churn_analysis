# Customer Churn Analysis

## Project Description

This project analyzes customer churn for a telecommunications company using SQL, statistical hypothesis testing, and machine-learning models. Its purpose is to identify churn patterns, predict customers at risk, and recommend practical retention strategies.

## Business Problem

Customer churn reduces recurring revenue and can increase customer acquisition costs. The company needs to identify the customer characteristics associated with churn and prioritize customers for retention interventions.

## Data Source

The project uses IBM's Telco Customer Churn dataset:

[raw.githubusercontent.com](https://raw.githubusercontent.com/IBM/telco-customer-churn-on-icp4d/master/data/Telco-Customer-Churn.csv)

## Approach

The analysis includes:

- Data inspection and cleaning with Pandas
- SQLite queries for customer segmentation and churn rates
- Descriptive statistics and visualizations
- A chi-square test of Contract and Churn
- A Welch independent-samples t-test of MonthlyCharges by Churn
- Logistic Regression, Decision Tree, and Random Forest models
- Evaluation using accuracy, precision, recall, F1, and confusion matrices
- Random Forest feature-importance analysis

## Key Findings

- Contract type showed a statistically significant association with churn.
- Churn patterns varied across contract and internet-service categories.
- Tenure, charges, contract characteristics, and service-related variables contributed to churn prediction.
- The highest-accuracy model was **[MODEL]**, with test accuracy of **[VALUE]**.
- The highest-F1 model was **[MODEL]**, with an F1 score of **[VALUE]**.

## Business Recommendations

- Prioritize customers with high predicted churn risk.
- Test incentives for month-to-month customers to move to longer contracts.
- Improve onboarding and early-tenure customer support.
- Offer plan reviews to high-risk customers with high monthly charges.
- Evaluate retention campaigns through controlled experiments.

## Tools Used

- Python
- Pandas
- NumPy
- SQLite
- SciPy
- Scikit-learn
- Matplotlib
- Seaborn
- Google Colab
- GitHub

## Repository Files

- `customer_churn_analysis.ipynb`: Complete analysis and model development
- `queries.sql`: All SQL queries used in the analysis
- `Telco-Customer-Churn-cleaned.csv`: Optional cleaned dataset

## How to Run

1. Download or clone this repository.
2. Open `customer_churn_analysis.ipynb` in Jupyter Notebook or Google Colab.
3. Run the cells from top to bottom.
4. An internet connection is required when loading the source dataset from its URL.
