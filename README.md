# Customer-Churn-Prediction-Using-Neural-Networks-ANN-

📌 Project Overview

This project focuses on predicting customer churn using a Deep Learning model (Artificial Neural Network) built with TensorFlow/Keras. The goal is to identify customers likely to leave a telecom service based on their usage patterns, account details, and billing information.

🎯 Objectives

Predict whether a customer will churn
Perform data preprocessing and feature engineering
Build and train a neural network model
Evaluate model performance for business insights

📂 Dataset

The dataset includes:

Customer demographics (gender, partner, dependents)
Account details (tenure, contract type)
Services subscribed (internet, phone, streaming, etc.)
Billing information (monthly & total charges)

🔍 Exploratory Data Analysis (EDA)

Removed invalid entries in TotalCharges
Converted TotalCharges to numeric format
Visualized churn distribution using histograms
Compared Monthly Charges vs Churn
Analyzed feature patterns affecting churn

⚙️ Data Preprocessing

Handled missing/blank values
Converted categorical variables:
Yes/No → 1/0
Gender → binary encoding
Applied One-Hot Encoding using pd.get_dummies()
Scaled numerical features (tenure, MonthlyCharges, TotalCharges) using MinMaxScaler
Split dataset into training and testing sets (80/20)

🧠 Model Architecture

A simple Artificial Neural Network (ANN) was implemented:

Input Layer: 26 features
Hidden Layer:
Dense layer with 20 neurons (ReLU activation)
Output Layer:
1 neuron (Sigmoid activation for binary classification)

⚙️ Compilation & Training

Optimizer: Adam
Loss Function: Binary Crossentropy
Metrics: Accuracy
Epochs: 50
Batch Size: 2
Validation Split: 20%

📈 Results

The model successfully learned patterns in customer behavior
Achieved good accuracy on training and validation data
Identified key churn indicators such as:
Monthly charges
Tenure
Service usage

🚀 Tech Stack

Python
TensorFlow / Keras
Pandas, NumPy
Matplotlib
Scikit-learn

📌 Future Improvements

Implement CNN or advanced deep learning architectures
Perform hyperparameter tuning
Handle class imbalance using SMOTE or class weights
Deploy model using Streamlit or Flask

📎 Conclusion

This project demonstrates how a basic neural network can be used to predict customer churn and uncover important business insights that help improve customer retention.
