# Customer Churn Prediction

Predicting whether a customer will churn using Machine Learning models.

---

## Project Overview

Customer churn is a major problem in subscription-based businesses.  
This project builds a machine learning model to predict whether a customer is likely to leave the service.

---

## Dataset

- Total Records: 3328
- Features: 
  - State
  - Account Length
  - Area Code
  - Phone
  - Int'l Plan
  - VMail Plan
  - VMail Message
  - Day Minutes
  - Day Calls
  - Day Charge
  - Eve Minutes
  - Eve Calls
  - Eve Charge
  - Night Minutes
  - Night Calls
  - Night Charge
  - Intl Minutes
  - Intl Calls
  - Intl Charge
  - CustServ Calls
  - Churn?

---

## Tech Stack

- Pandas
- NumPy
- Matplotlib & Seaborn
- Scipy

---

## Data Preprocessing

- **Removed Unnamed Columns** – Dropped automatically generated index columns that had no analytical value.

- **Identified Outliers** – Checked numerical features for extreme values that could distort model performance.

- **Handled Missing Values** – Removed or cleaned rows containing null values to maintain data consistency.

- **Cleaned Numeric Columns** – Converted numeric columns containing string values into proper numerical format.

- **Cleaned Categorical Columns** – Ensured string columns did not contain incorrect numeric values.

- **Removed Irrelevant Data** – Eliminated inconsistent or invalid rows to improve data quality. Ensured column contained only valid categorical values (`yes` and `no`)/(`True.` and `False.`)

- **Encoded Categorical Variables** – Converted categorical variables into numerical format using mapping


## Exploratory Data Analysis (EDA)

- **Distribution of Churn** – Analyzed the distribution of the target variable `Churn?` to understand the class imbalance.

- **Correlation Matrix** – Visualized the correlation between numerical features using a heatmap to identify multicollinearity.

- **Pairwise Relationships** – Examined pairwise relationships between numerical features using a scatter matrix to understand their interactions.

- **Distribution Analysis (Histograms)** – Analyzed the distribution of numerical features using histograms to understand their distribution.

- **Outlier Detection (Boxplots)** – Detected outliers in numerical features using boxplots to understand their distribution.

---

## Models Used

- Decision Tree
- Naive Bayes
- Random Forest

---

## Model Performance Comparison

| Split Method | Accuracy | F1 Score | Recall | Precision |
|--------------|----------|----------|--------|-----------|
| Simple Train-Test (Decision Tree) | 0.9383 | 0.8122 | 0.7917 | 0.7835 |
| K-Fold (k=10) (Decision Tree) | 0.9201 | 0.7141 | 0.7261 | 0.7246 |
| K-Fold (k=3) (Decision Tree) | 0.9105 | 0.7004 | 0.7137 | 0.6839 |
| Simple Train-Test (Naive Bayes) | 0.8765 | 0.5119 | 0.4479 | 0.5972 |
| K-Fold (k=10) (Naive Bayes) | 0.8532 | 0.4631 | 0.4357 | 0.4941 |
| K-Fold (k=3) (Naive Bayes) | 0.8541 | 0.4670 | 0.4398 | 0.4977 |
| Simple Train-Test (Random Forest) | 0.9593 | 0.8421 | 0.7500 | 0.9600 |
| K-Fold (k=10) (Random Forest) | 0.9536 | 0.8205 | 0.7303 | 0.9362 |
| K-Fold (k=3) (Random Forest) | 0.9524 | 0.8119 | 0.7075 | 0.9525 |
---

## Key Insights

- Customers with month-to-month contracts churn more.
- Higher monthly charges increase churn probability.
- Long-term customers are less likely to churn.

---

## How to Run the Project

1. Clone the repository
2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Open Jupyter Notebook:

```bash
jupyter notebook
```

4. Run `Customer Churn.ipynb`

---

## Future Improvements

- Hyperparameter tuning
- Deployment using Streamlit
- Model explainability using SHAP

---

## Author

Saachi Garg  
MSc Data Science  

Dhirubhai Ambani University
