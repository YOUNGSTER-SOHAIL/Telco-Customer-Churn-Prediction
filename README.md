# Telco-Customer-Churn-Prediction
This project predicts customer churn using an extended Telco dataset. It includes preprocessing, EDA, and ML models (Logistic Regression, Random Forest, Gradient Boosting, SVM). Logistic Regression achieved ~80% accuracy and 0.85 AUC. The framework is adaptable to telecom, banking, and healthcare.
Telco Customer Churn Prediction

Overview:
Customer churn is a major challenge across industries such as telecommunications, banking, finance, and healthcare. Churn occurs when customers discontinue using a service, leading to revenue loss. This project develops a machine learning pipeline to predict customer churn using an extended version of the IBM Telco Customer Churn dataset.

The task is framed as a binary classification problem where:

0 → Customer stays

1 → Customer churns

Objectives:

Perform data preprocessing and handle missing values.

Conduct exploratory data analysis (EDA) to identify churn drivers.

Build and compare multiple machine learning models.

Evaluate models with multiple performance metrics.

Save the best model for deployment.

Workflow:

1. Data Preprocessing

Converted categorical variables with OneHotEncoder

Scaled numerical features using StandardScaler

Filled missing TotalCharges values with median

Removed duplicates and irrelevant columns

2. Exploratory Data Analysis (EDA)

Checked churn distribution (class imbalance ~26% churn vs 74% non-churn)

Visualized key features: tenure, monthly charges, contract type, payment method

Used correlation heatmaps and boxplots to find important predictors

3. Model Building

Trained and evaluated:

Logistic Regression

Random Forest

Gradient Boosting

Support Vector Machine (SVM)

4. Evaluation Metrics

Accuracy

Precision

Recall

F1-score

ROC-AUC

ROC curve plotted for best model (Logistic Regression)

Results:

Logistic Regression was the best-performing model with:

Accuracy: ~80%

ROC-AUC: 0.85

Ensemble models (Random Forest, Gradient Boosting) also performed competitively but Logistic Regression offered better balance and interpretability.

Deployment:

The best model (Logistic Regression) was saved along with preprocessing steps using joblib, enabling future predictions on new customer data.

Conclusion:

This project demonstrates a complete end-to-end churn prediction pipeline, from data preprocessing and EDA to model training and evaluation. While built on a telecom dataset, the framework is easily adaptable to banking, finance, and healthcare domains, making it highly practical for real-world retention analysis.
