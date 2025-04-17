# Telco Customer Churn Prediction

## Project Overview

This project aims to analyze customer churn in the telecom industry using a dataset from Kaggle. It utilizes data manipulation, visualization, and machine learning techniques to predict customer churn and identify key factors contributing to it.

**Domain:** Telecom

**Domain Context:**
Customer churn refers to customers discontinuing their services with a company. It's a critical challenge in the telecom industry. This project employs predictive analysis to understand the reasons behind customer churn and identify potential churners, enabling proactive measures to retain them.

**Lab Environment:** Google Colab (Hosted Jupyter Notebook service)

## Data Manipulation

The project performs the following data manipulation tasks:

1.  Calculates the total number of male customers.
2.  Determines the total number of customers with DSL internet service.
3.  Identifies female senior citizens using mailed check payments and stores them in a separate dataset.
4.  Extracts customers with tenure less than 10 months or total charges less than $500.
5.  Performs data type conversions and handles missing values in the dataset.

## Data Visualization

The project visualizes data using the following charts:

1.  **Pie Chart:** Shows the distribution of customers who churn.
2.  **Bar Plot:** Illustrates the distribution of different internet services.

## Model Building

The project builds three sequential models using Keras to predict customer churn:

**Model 1:**
*   Uses 'tenure' as the feature and 'Churn' as the target.
*   Includes an input layer with 12 nodes and ReLU activation.
*   Has a hidden layer with 8 nodes and ReLU activation.
*   Employs the Adam optimizer.
*   Trains for 150 epochs.
*   Evaluates performance with a confusion matrix and accuracy score.
*   Plots accuracy against epochs.

**Model 2:**
*   Similar to Model 1 but adds dropout layers (0.3 after input and 0.2 after the hidden layer) to prevent overfitting.
*   Evaluates performance and plots accuracy.

**Model 3:**
*   Uses 'Tenure', 'Monthly Charges', and 'Total Charges' as features.
*   Follows a similar structure to Model 1 with an input layer, hidden layer, and output layer.
*   Evaluates performance and plots accuracy.

## How to Run the Project

1.  Open the Jupyter Notebook in Google Colab.
2.  Install necessary libraries using `!pip install library_name`.
3.  Execute the code cells sequentially.
4.  Review the results and visualizations.

## Conclusion

This project provides insights into customer churn and demonstrates the use of machine learning models for churn prediction. The models can assist telecom companies in identifying potential churners and taking preventive actions.
