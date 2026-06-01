# Loan Default Prediction using Machine Learning

## Project Overview

This project focuses on predicting whether a customer is likely to default on a loan using machine learning techniques. The project includes complete data preprocessing, exploratory data analysis (EDA), model training, evaluation, and feature importance analysis.

The main objective was to understand the end-to-end machine learning workflow and compare different classification models on an imbalanced financial dataset.

---

## Dataset Information

* Total Rows: 252,000
* Features: Income, Age, Experience, Profession, House Ownership, State, City, etc.
* Target Variable: `Risk_Flag`

  * `0` → Safe Customer
  * `1` → Risky Customer

The dataset was highly imbalanced, making model evaluation more challenging.

---

## Project Workflow

### 1. Exploratory Data Analysis (EDA)

* Checked dataset structure and data types
* Analyzed numerical and categorical features
* Visualized feature distributions
* Identified class imbalance
* Created correlation heatmaps

### 2. Data Preprocessing

* Removed unnecessary columns (`Id`)
* Applied One-Hot Encoding to categorical features
* Split dataset into training and testing sets
* Handled imbalanced data using class weights

### 3. Model Training

The following machine learning models were trained and evaluated:

* Logistic Regression
* Decision Tree Classifier
* Random Forest Classifier

### 4. Model Evaluation

Models were evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix

Special focus was given to Recall because correctly identifying risky customers is important in loan default prediction.

---

## Results Summary

| Model               | Accuracy | Recall (Risky Customers) |
| ------------------- | -------- | ------------------------ |
| Logistic Regression | 65%      | 31%                      |
| Decision Tree       | 88%      | 82%                      |
| Random Forest       | 89%      | 76%                      |

Random Forest achieved the best overall performance with strong balance between accuracy and risky customer detection.

---

## Feature Importance

Top important features identified by Random Forest:

* Income
* Age
* Experience
* Current Job Years
* Current House Years
* Car Ownership
* State Information

These features contributed the most to predicting loan default risk.

---

## Key Learnings

Through this project, the following machine learning concepts were learned:

* Exploratory Data Analysis (EDA)
* Feature Encoding
* Handling Imbalanced Data
* Train-Test Split
* Logistic Regression
* Decision Trees
* Random Forest
* Overfitting vs Underfitting
* Ensemble Learning
* Model Evaluation Metrics
* Feature Importance Analysis

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Joblib
* Jupyter Notebook

---

## Project Structure

```text
loan-default-predictor/
│
├── data/
├── notebooks/
├── models/
├── images/
├── requirements.txt
└── README.md
```

---

## Future Improvements

Possible future improvements for this project:

* Hyperparameter Tuning
* SMOTE for imbalance handling
* XGBoost implementation
* Model deployment using Flask or Streamlit
* Cross-validation

---

## Conclusion

This project provided a strong understanding of the complete machine learning workflow from preprocessing to model evaluation. It also demonstrated the importance of handling imbalanced datasets and selecting appropriate evaluation metrics for financial prediction problems.
