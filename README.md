# Customer Churn Prediction & Analysis

##  Overview
This project focuses on predicting customer churn using machine learning techniques.
The goal is to identify customers who are likely to leave and analyze the key factors
influencing churn.

##  Dataset
- Dataset contains 7,000+ customer records
- Includes features like customer demographics, services, and account information
- **Source:** Telco Customer Churn — Kaggle
- **Target variable:** Churn (Yes/No) | **Churn Rate:** 26.5%

##  Approach

### 🔹 Data Preprocessing
- Handled missing values and cleaned dataset
- Performed feature encoding for categorical variables
- Scaled numerical features for model training

### 🔹 Exploratory Data Analysis (EDA)
- Analyzed churn distribution and class imbalance
- Identified key features affecting churn behavior

### 🔹 Handling Class Imbalance
- Applied **SMOTE** (Synthetic Minority Oversampling Technique)
- Improved model's ability to detect churn customers

##  Model Building

**Models Used:**
- Logistic Regression
- Random Forest

**Final Model:**
- Logistic Regression (better performance on recall)

##  Model Evaluation

| | Before SMOTE | After SMOTE |
|---|---|---|
| **Accuracy** | ~82% | ~79% |
| **Recall (Churn)** | ~60% | ~68% |

- Reduced false negatives significantly

**Metrics Used:**
- Accuracy, Precision, Recall, F1-Score, Confusion Matrix, ROC-AUC

##  Key Insights
- Model improved churn detection by reducing missed churn cases (~20%)
- Trade-off observed between accuracy and recall due to class imbalance
- Fiber optic users and month-to-month contract customers churn the most
- Identified importance of focusing on **Recall** for business impact

##  Tools & Technologies
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
- Imbalanced-learn (SMOTE)
- Google Colab


##  Conclusion
The project demonstrates how handling class imbalance and focusing on appropriate
evaluation metrics can significantly improve model performance for real-world business
problems. Recall matters more than accuracy when identifying churners.
