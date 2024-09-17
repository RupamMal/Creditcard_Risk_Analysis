Credit Risk Analysis Using Machine Learning
Overview
This project applies machine learning techniques to predict credit risk for a peer-to-peer lending services company, Fast Lending. Accurate credit risk prediction helps identify good candidates for loans, reduces default rates, and improves overall lending decisions. Several resampling techniques and ensemble classifiers are used to handle class imbalances in the data and improve prediction accuracy.

Table of Contents
Project Overview
Goals and Objectives
Data
Project Structure
Models and Methods
Results
Installation and Requirements
Usage
Contributing
License
Goals and Objectives
The main objectives of this project are:

Use Resampling Models to Predict Credit Risk
Utilize resampling methods such as Random Over-Sampling, SMOTE, and Cluster Centroids to balance the training data and apply Logistic Regression for initial predictions.

Use the SMOTEENN Algorithm
Implement the SMOTEENN algorithm, which combines both over- and under-sampling techniques to generate balanced datasets, and use Logistic Regression for prediction.

Apply Ensemble Classifiers
Use advanced machine learning models such as the Balanced Random Forest Classifier and Easy Ensemble AdaBoost Classifier to reduce bias and improve model performance.

Evaluate Models and Provide Recommendations
Compare the results of different models based on accuracy, precision, recall, F1-score, and other performance metrics, and make recommendations for the best-performing model.

Data
The dataset used in this project is from LendingClub, a peer-to-peer lending services company. The dataset contains historical loan data that includes features such as loan amount, credit score, and payment history. The goal is to predict the likelihood of a borrower defaulting on a loan.

Data Source: LoanStats_2019Q1.rar
Jupyter Notebooks:
credit_risk_resampling.ipynb
credit_risk_ensemble.ipynb
Project Structure
kotlin
Copy code
├── data
│   └── LoanStats_2019Q1.rar
├── notebooks
│   ├── credit_risk_resampling.ipynb
│   ├── credit_risk_ensemble.ipynb
├── README.md
└── LICENSE
notebooks/: Contains the Jupyter Notebooks used for analysis.
data/: The dataset from LendingClub.
Models and Methods
Resampling Methods:

Random Over-Sampler
SMOTE (Synthetic Minority Over-sampling Technique)
Cluster Centroids
SMOTEENN (Combining SMOTE and Edited Nearest Neighbors)
Machine Learning Algorithms:

Logistic Regression: Used as a baseline classifier.
Balanced Random Forest Classifier: An ensemble method that addresses class imbalance.
Easy Ensemble AdaBoost Classifier: An ensemble method that reduces bias and improves performance.
Performance Evaluation:

Accuracy Score
Confusion Matrix
Precision, Recall, F1-Score
Feature Importance (for Balanced Random Forest Classifier)
Results
Model	Balance Accuracy Score
Random Over Sampler (Logistic Regression)	0.6835
SMOTE Oversampling (Logistic Regression)	0.6277
Cluster Centroids (Logistic Regression)	0.5297
SMOTEENN (Logistic Regression)	0.6548
Balanced Random Forest Classifier	0.8731
Easy Ensemble AdaBoost Classifier	0.9424
Summary
The Easy Ensemble AdaBoost Classifier performed the best with a balanced accuracy score of 0.9424, and it showed the highest precision and recall metrics. This model is recommended for predicting credit risk due to its robustness in handling imbalanced data and delivering accurate predictions.

Installation and Requirements
Requirements
Python 3.8.8 or later
Visual Studio Code 1.64.2
Jupyter Notebook 6.4.8
pandas 1.4.1
numpy 1.20.3
scikit-learn 1.0.2
Installation
Clone the repository:

bash
Copy code
git clone https://github.com/your-username/credit-risk-analysis.git
cd credit-risk-analysis
Install the required packages:

bash
Copy code
pip install -r requirements.txt
Open the Jupyter Notebook:

bash
Copy code
jupyter notebook
Usage
Run the credit_risk_resampling.ipynb notebook to apply different resampling techniques and evaluate model performance.
Run the credit_risk_ensemble.ipynb notebook to evaluate the ensemble classifiers (Balanced Random Forest and Easy Ensemble AdaBoost).
Analyze the results and compare model performance to decide on the best approach for credit risk prediction.
Contributing
Contributions are welcome! If you'd like to contribute, please fork the repository and make a pull request with detailed notes on the changes you made.

License
This project is licensed under the MIT License - see the LICENSE file for details.
