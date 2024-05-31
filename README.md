# Titanic Survival Prediction

## Overview

This project aims to predict the survival of passengers on the Titanic using a machine learning model. The model is built using the Titanic dataset from Kaggle and employs logistic regression for the predictions. Additionally, a web interface is provided to allow users to input passenger data and get survival predictions.

## Dataset

The dataset used for this project is available on Kaggle: [Titanic Dataset](https://www.kaggle.com/datasets/yasserh/titanic-dataset).

## Libraries and Tools

- **NumPy**: For numerical operations.
- **Pandas**: For data manipulation and analysis.
- **Scikit-Learn**: For building and evaluating the machine learning model.
- **Flask**: For creating the web application.
- **pyngrok**: For exposing the local Flask app to the internet.

## Steps Involved

### 1. Data Loading

The Titanic dataset is loaded from Kaggle using pandas.

### 2. Data Preprocessing

- Missing and null values are handled by either removing or replacing them.
- Categorical data is encoded to numerical values.

### 3. Data Analysis and Visualization

Data is analyzed to understand the distribution of survival based on different features. Visualization tools are used to present the analysis.

### 4. Model Building

The model used for prediction is Logistic Regression.

**Logistic Regression**: It is a statistical method for analyzing a dataset with one or more independent variables that determine an outcome.

### 5. Model Evaluation

The model is evaluated using training and testing data.

### 6. Model Deployment

The trained model is saved using `joblib` for later use.

### 7. Web Application

A web application is created using Flask to allow users to input passenger details and get survival predictions.

#### Flask Application

- **Home Route** (`/`): Displays a form for inputting passenger data.
- **Predict Route** (`/predict`): Takes the form data, processes it, and returns a survival prediction.

### 8. ngrok Integration

`pyngrok` is used to expose the local Flask application to the internet, providing a public URL.

## Running the Application

1. **Install Dependencies**:
   
   ```bash
   pip install numpy pandas scikit-learn flask pyngrok joblib


2. **Load the trained model and initialize the Flask app.**

Define routes for the home page (/) and prediction (/predict).

Start the Flask app on localhost.
**Access the Application**:

Use the public URL provided by ngrok to access the web application.

## Conclusion
This project demonstrates how to build and deploy a machine learning model for predicting Titanic survival using logistic regression. The web application allows for easy interaction and provides real-time predictions based on user inputs.

## References

- Kaggle Titanic Dataset: [Titanic Dataset](https://www.kaggle.com/datasets/yasserh/titanic-dataset)
- Scikit-Learn Documentation: [Scikit-Learn](https://scikit-learn.org/stable/)
