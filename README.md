# Customer Churn Prediction and Customer Segmentation

## 📌 Project Overview

Customer churn is one of the biggest challenges faced by telecom companies. This project uses Machine Learning to predict whether a customer is likely to leave the company (Churn Prediction) and also groups customers into different categories using Customer Segmentation.

The project includes data preprocessing, exploratory data analysis (EDA), feature engineering, machine learning model building, model evaluation, and customer segmentation using K-Means clustering.

---

# 📖 Table of Contents

- Project Overview
- Problem Statement
- Objectives
- Dataset
- Technologies Used
- Project Workflow
- Exploratory Data Analysis
- Data Preprocessing
- Feature Engineering
- Machine Learning Model
- Handling Class Imbalance
- Hyperparameter Tuning
- Feature Importance
- Customer Segmentation
- Model Evaluation
- Results
- Future Improvements
- Folder Structure
- How to Run
- Author

---

# 🎯 Problem Statement

Telecommunication companies lose customers due to better offers from competitors. Predicting customer churn helps companies identify customers who are likely to leave and allows them to take preventive actions.

This project predicts customer churn and segments customers based on their behavior for better business decisions.

---

# 🎯 Objectives

- Predict customer churn using Machine Learning.
- Analyze customer behavior.
- Identify important features affecting churn.
- Improve prediction performance using Random Forest.
- Segment customers into meaningful groups using K-Means Clustering.

---

# 📂 Dataset

Dataset Used:

**Telco Customer Churn Dataset**

The dataset contains customer information such as:

- Customer ID
- Gender
- Senior Citizen
- Partner
- Dependents
- Tenure Months
- Phone Service
- Internet Service
- Contract Type
- Payment Method
- Monthly Charges
- Total Charges
- Churn Value
- Churn Label

Target Variable:

**Churn Value**

- 1 → Customer Left
- 0 → Customer Stayed

---

# 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

---

# 🔄 Project Workflow

1. Import Libraries
2. Load Dataset
3. Data Exploration
4. Data Cleaning
5. Feature Encoding
6. Train-Test Split
7. Random Forest Classification
8. Hyperparameter Tuning
9. Feature Importance Analysis
10. Customer Segmentation using K-Means
11. Model Evaluation

---

# 📊 Exploratory Data Analysis (EDA)

The following analyses were performed:

- Distribution of Tenure Months
- Distribution of Monthly Charges
- Contract vs Churn
- Internet Service vs Churn
- Payment Method vs Churn
- Tech Support vs Churn
- Correlation Matrix
- Average Tenure Analysis

Several visualizations were created using Matplotlib and Seaborn.

---

# 🧹 Data Preprocessing

The following preprocessing steps were performed:

- Converted Total Charges into numeric format
- Filled missing values
- Removed unnecessary columns
- One-Hot Encoding using Pandas
- Feature Selection

Dropped columns include:

- CustomerID
- Country
- State
- City
- Latitude
- Longitude
- Zip Code
- Churn Label
- Churn Score
- CLTV
- Churn Reason

---

# ⚙ Feature Engineering

Categorical features were converted into numerical format using One-Hot Encoding.

The final feature set was used for training the Random Forest classifier.

---

# 🤖 Machine Learning Model

Algorithm Used:

## Random Forest Classifier

Why Random Forest?

- Handles high-dimensional data
- Reduces overfitting
- Provides Feature Importance
- High prediction accuracy

---

# ⚖ Handling Class Imbalance

To improve prediction performance, the Random Forest model was trained using:

```
class_weight="balanced"
```

This helps the model learn equally from both churned and non-churned customers.

---

# 🔧 Hyperparameter Tuning

The tuned Random Forest model uses:

- Number of Trees = 300
- Maximum Depth = 10
- Balanced Class Weight

This improves model performance and generalization.

---

# 📈 Feature Importance

Feature Importance analysis was performed to identify the most influential variables affecting customer churn.

Less important features were removed to simplify the model.

---

# 👥 Customer Segmentation

After predicting churn probability, customers were segmented using **K-Means Clustering**.

Three customer groups were created:

### 1. Budget Loyal Customers

- Low Monthly Charges
- Long Tenure
- Low Churn Probability

### 2. High Risk Customers

- High Churn Probability
- Likely to leave the company

### 3. Loyal Premium Customers

- High Monthly Charges
- Long-Term Customers
- Valuable customers

---

# 📊 Model Evaluation

Evaluation Metrics Used:

- Accuracy
- Confusion Matrix
- Precision
- Recall
- F1 Score
- ROC Curve

These metrics were used to evaluate the performance of the Random Forest classifier.

---

# 📌 Results

✔ Customer churn prediction achieved good classification performance.

✔ Important features affecting churn were successfully identified.

✔ Customers were segmented into three meaningful business groups.

✔ The model can help telecom companies reduce customer loss through targeted retention strategies.

---

# 🚀 Future Improvements

- Deploy the model using Streamlit or Flask
- Use XGBoost or LightGBM
- Perform Cross Validation
- Add Deep Learning models
- Create a Dashboard using Power BI

---

# 📁 Folder Structure

```
CustomerChurn/
│
├── CBSOTPROJ1.ipynb
├── Telco_customer_churn.xlsx
├── README.md
```


# 📚 Libraries Used

- pandas
- numpy
- matplotlib
- seaborn
- sklearn

---


Machine Learning | Data Science | Python
