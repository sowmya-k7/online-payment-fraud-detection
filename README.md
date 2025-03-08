# online-payment-fraud-detection
Summary of Online Payment Fraud Detection
The provided code is a Python-based online payment fraud detection system that leverages machine learning techniques for fraud classification. Below is an overview of its key components:

1. Data Preprocessing
The dataset is read using Pandas (pd.read_csv).
Basic data exploration is performed using .info(), .describe(), and .head().
Missing values and fraud-related attributes (isFraud, isFlaggedFraud) are analyzed.
Categorical data (Transaction Type) is mapped to numerical values for better processing.
2. Exploratory Data Analysis (EDA)
The correlation between features and fraud occurrences is analyzed using Seaborn & Plotly.
Transaction types (CASH_OUT, PAYMENT, TRANSFER, etc.) are visualized using a pie chart.
Irrelevant columns like nameOrig and nameDest are removed.
3. Data Splitting and Resampling
The dataset is balanced to handle the class imbalance between fraud and non-fraud transactions.
The data is split into training, validation, and testing sets using train_test_split().
4. Fraud Detection Models
Two machine learning models are trained and evaluated:
Decision Tree Classifier
Random Forest Classifier
5. Hyperparameter Tuning (GridSearchCV)
Both models undergo hyperparameter tuning using GridSearchCV to optimize:
criterion (gini, entropy, log_loss)
max_depth
max_features
n_estimators (for Random Forest)
6. Performance Evaluation
The models are assessed using:
Precision-Recall Curves
ROC Curves
AUC Scores
Confusion Matrices
Classification Reports (Precision, Recall, F1-Score)
7. Results
The Decision Tree and Random Forest models are compared based on AUC and classification reports.
Random Forest generally provides better accuracy and fraud detection performance.
