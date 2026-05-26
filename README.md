# Customer Churn Prediction

A machine learning project focused on predicting customer churn using customer behavior and service usage data. This project applies data preprocessing, exploratory data analysis (EDA), class imbalance handling, and machine learning models to identify customers who are likely to leave a service.

---

## Project Overview

Customer churn prediction helps businesses identify customers who are at risk of leaving their service. By analyzing customer demographics, subscription details, payment methods, and usage patterns, machine learning models can predict churn and support customer retention strategies.

This project includes:

- Data preprocessing and cleaning
- Exploratory Data Analysis (EDA)
- Feature engineering and encoding
- Handling class imbalance using SMOTE
- Model training and evaluation
- Performance comparison of classification algorithms

---

## Dataset

The dataset contains customer-related information such as:

- Customer demographics
- Tenure
- Internet service details
- Contract type
- Payment method
- Monthly and total charges
- Churn status

Target Variable:

- `Churn`
  - `1` → Customer churned
  - `0` → Customer retained

---

## Technologies Used

### Programming Language
- Python

### Libraries
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Imbalanced-learn (SMOTE)

---

## Project Workflow

### 1. Data Loading
- Imported the customer churn dataset
- Examined dataset structure and feature types

### 2. Data Preprocessing
- Removed unnecessary columns such as `customerID`
- Converted `TotalCharges` to numeric format
- Handled missing values using median imputation
- Encoded target labels using `LabelEncoder`
- Applied one-hot encoding to categorical variables

### 3. Exploratory Data Analysis (EDA)

Performed visual analysis to understand churn behavior:

- Churn distribution analysis
- Tenure vs churn relationship
- Monthly charges vs churn
- Contract type analysis
- Internet service analysis
- Payment method analysis

### Key Insights

- Customers with month-to-month contracts are more likely to churn
- Higher monthly charges are associated with higher churn probability
- New customers show higher churn risk
- Electronic check users exhibit higher churn rates
- Long-term customers are less likely to churn

---

## Handling Class Imbalance

The dataset showed imbalance between churned and non-churned customers.

To address this:

- Applied **SMOTE (Synthetic Minority Oversampling Technique)**
- Balanced the target classes before model training

---

## Machine Learning Models

The following classification models were implemented:

### Logistic Regression
- Baseline classification model
- Evaluated before and after SMOTE

### Random Forest Classifier
- Ensemble learning approach
- Improved prediction performance

### Decision Tree Classifier
- Tree-based classification model
- Easy model interpretability

---

## Model Evaluation Metrics

The models were evaluated using:

- Accuracy Score
- Precision
- Recall
- F1-Score
- Confusion Matrix
- Classification Report

---

## Results

The project demonstrates that handling class imbalance and selecting relevant customer behavior features significantly improves churn prediction performance.

Among the tested models, ensemble-based methods such as Random Forest generally produced stronger predictive performance.

---

## Project Structure

```bash
Customer-Churn-Prediction/
│
├── Customer_Churn_Prediction_Project.ipynb
├── README.md
└── dataset.csv
```

---


## Future Improvements

- Hyperparameter tuning
- Feature selection optimization
- Deployment using Flask or Streamlit
- Real-time churn prediction dashboard
- Deep learning approaches for improved accuracy

---

## Conclusion

This project provides a complete end-to-end workflow for customer churn prediction using machine learning. It highlights the importance of preprocessing, exploratory data analysis, and class balancing techniques in improving classification performance.

---

## Author

Developed as a machine learning project for customer churn analysis and predictive modeling.

