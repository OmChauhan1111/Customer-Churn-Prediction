# Customer Churn Prediction

## Project Overview
Customer churn prediction is a critical task for businesses to identify customers who are likely to leave their services. This project builds a machine learning model to predict whether a customer will churn based on their account information and behavior. The goal is to help businesses proactively retain valuable customers by understanding churn drivers.

---

## Dataset
The dataset used is the **Telco Customer Churn** dataset sourced from [Kaggle](https://www.kaggle.com/blastchar/telco-customer-churn). It contains customer demographics, account details, service usage, and whether the customer churned.

**Dataset size:** ~7,000 rows and 21 columns  
**Target variable:** `Churn` (Yes/No)

---

## Objective
- Predict customer churn (binary classification: churn vs. no churn).
- Identify key features that contribute most to customer churn.
- Evaluate the model performance using accuracy, precision, recall, and F1-score.

---

## Technologies & Libraries Used
- Python 3.x
- pandas, numpy (for data manipulation)
- matplotlib, seaborn (for data visualization)
- scikit-learn (for machine learning and model evaluation)

---

## Methodology

### 1. Data Loading and Cleaning
- Loaded the CSV dataset into a pandas DataFrame.
- Checked for missing values and handled them.
- Converted the `TotalCharges` column to numeric, filling missing values with median.

### 2. Exploratory Data Analysis (EDA)
- Visualized churn distribution.
- Analyzed categorical and numerical features.

### 3. Data Preprocessing
- Dropped irrelevant columns (e.g., `customerID`).
- Encoded categorical variables using Label Encoding.
- Converted the target column `Churn` to binary (Yes=1, No=0).
- Scaled numeric features using StandardScaler.

### 4. Model Building
- Split data into training (80%) and testing (20%) sets.
- Trained a Random Forest classifier on the training data.
- Predicted churn on the test data.

### 5. Evaluation
- Evaluated model using:
  - Accuracy
  - Precision
  - Recall
  - F1-score
- Visualized results with a confusion matrix.
- Plotted feature importance to identify top churn drivers.

---

## How to Run the Project

### Prerequisites
- Python 3.x installed
- Required libraries installed. You can install them using:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
