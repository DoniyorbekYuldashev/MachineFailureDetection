Machine Failure Detection
Project Overview
The Machine Failure Detection project predicts machine failures in industrial settings using sensor data, enabling predictive maintenance to minimize downtime. It uses machine learning to classify machines as likely to fail (1) or not (0) and predict failure probability via regression. The analysis is performed in a Jupyter notebook (MachineFailureDetection.ipynb) using a dataset with sensor measurements (e.g., temperature, torque, tool wear) and evaluates models like Random Forest, XGBoost, and SVM.
Objectives

Build models to predict machine failures accurately.
Handle imbalanced data using SMOTE.
Compare classification and regression model performance.
Support predictive maintenance applications.

Dataset
The dataset includes 10,000 records with:

UDI, Product ID: Identifiers.
Type: Product type (L, M, H).
Air temperature [K], Process temperature [K]: Temperatures.
Rotational speed [rpm], Torque [Nm], Tool wear [min]: Operational metrics.
Machine failure: Target (0 = no failure, 1 = failure).
TWF, HDF, PWF, OSF, RNF: Failure modes.

The dataset is imbalanced, addressed using SMOTE in the notebook.
Notebook Content
The notebooks/MachineFailureDetection.ipynb includes:

Data Preprocessing: Cleaning, encoding categorical variables, scaling features.
Exploratory Data Analysis: Visualizing feature distributions and correlations.
Models:
Classification: Random Forest, Decision Tree, SVM, Naive Bayes, XGBoost.
Regression: Linear Regression, Decision Tree, Random Forest, SVR, XGBoost.


Evaluation: Accuracy, precision, recall, F1-score; MSE, R².
SMOTE: Balances failure/non-failure classes.
Hyperparameter Tuning: Optimizes Random Forest performance.

Setup and Usage
Prerequisites

Python 3.8+
Git
Jupyter Notebook

Installation

Clone the Repository:
git clone https://github.com/your-username/machine-failure-detection.git
cd machine-failure-detection


Create a Virtual Environment (optional):
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

Install Dependencies:
pip install -r requirements.txt

Running the Notebook

Launch Jupyter Notebook:jupyter notebook


Open notebooks/MachineFailureDetection.ipynb and run the cells.

Dataset

The notebook assumes the dataset is loaded from a CSV file (e.g., machine_failure_data.csv).
Update the file path in the notebook to your dataset location.

Requirements
Listed in requirements.txt:

pandas
numpy
scikit-learn
xgboost
imbalanced-learn
matplotlib
seaborn
jupyter

Doniyor Yuldashev

Notes

The dataset is not included in the repository. Source it (e.g., from Kaggle) and update the notebook’s file path.
The notebook handles imbalanced data; review SMOTE application for optimal results."# MachineFailureDetection" 
