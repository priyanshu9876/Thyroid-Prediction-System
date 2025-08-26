Thyroid Disease Detection

Thyroid disease is a common health issue in India, affecting millions of people each year. Thyroid disorders can either speed up or slow down the body's metabolism, causing multiple health complications.

The main goal of this project is to predict if a person is suffering from compensated hypothyroid, primary hypothyroid, secondary hypothyroid, or no thyroid disorder (negative) using Machine Learning. Classification algorithms like Random Forest, XGBoost, and KNN have been trained on the UCI Thyroid Dataset. After hyperparameter tuning, XGBoost performed the best in terms of accuracy, precision, and recall. The application is deployed on Heroku using the Flask framework.


Technical Aspects

Python Version: 3.7 or above

Libraries: sklearn, pandas, numpy, matplotlib, seaborn

Front-end: HTML, CSS

Back-end: Flask

IDE: Jupyter Notebook, PyCharm, VSCode

Database: Cassandra

Deployment: Heroku, AWS

How to Run this App

Code is written in Python 3.7+. To run:

Install Python: Python Downloads

Create virtual environment:

conda create -n tdd_env python=3.7
conda activate tdd_env


Install required packages:

pip install -r requirements.txt


Run the app:

python app.py

Workflow
Data Collection

Thyroid Disease dataset from UCI Machine Learning Repository:
UCI Thyroid Dataset

Data Pre-processing

Handle missing values using KNN Imputer

Detect and remove outliers using boxplots and percentile method

Encode categorical features using ordinal encoding and label encoding

Feature scaling using Standard Scaler

Handle imbalanced dataset with SMOTE

Drop unnecessary columns

Model Creation and Evaluation

Tested various classification algorithms: Random Forest, XGBoost, KNN

XGBoost selected for final model due to best performance

Hyperparameter tuning using RandomizedSearchCV

Model performance evaluated using accuracy, confusion matrix, and classification report

Database Connection

Data and predictions stored in Cassandra Database for easy retrieval and analysis

Model Deployment

Flask backend deployed on Heroku for live predictions

User Interface
Single User Input Prediction

Users can input their parameters manually for prediction

Simple, intuitive design

UI Example (Placeholder):


Batch File Prediction
Homepage

Single-page interface to upload CSV files for batch predictions

Placeholder Image:


Upload CSV & Predict

Upload CSV → Click Predict → Get results


Author

Priyanshu Mishra
LinkedIn

Help Me Improve

If you find any bugs or issues, feel free to raise an issue. I will address it as soon as possible.
