# Ann-classification-Churn-Prediction


## Project Overview

Customer churn is a major challenge for businesses because losing existing customers can directly affect revenue and long-term growth. This project focuses on building an **Artificial Neural Network (ANN)-based machine learning application** to predict whether a customer is likely to leave a company.

The project uses customer-related information to train a deep learning classification model. The trained ANN learns patterns from historical customer data and predicts the probability of customer churn. This can help businesses identify customers who are at a higher risk of leaving and take preventive actions such as providing personalized offers, improving customer service, or introducing customer retention strategies.

## Objective

The main objective of this project is to develop a reliable binary classification model that can predict customer churn based on different customer attributes.

The project aims to:

* Analyze and preprocess customer data.
* Handle categorical and numerical features.
* Transform the input data into a format suitable for deep learning.
* Build an Artificial Neural Network using TensorFlow and Keras.
* Train the model to classify customers into churn and non-churn categories.
* Evaluate the performance of the trained model.
* Deploy the model as an interactive web application using Streamlit.

## Technology Stack

* **Python** – Programming language
* **Pandas** – Data manipulation and analysis
* **NumPy** – Numerical computations
* **Scikit-learn** – Data preprocessing and machine learning utilities
* **TensorFlow / Keras** – Building and training the ANN model
* **Matplotlib** – Data visualization
* **TensorBoard** – Monitoring model training
* **Streamlit** – Web application and deployment
* **Git & GitHub** – Version control and project hosting

## Model Architecture

The project uses a feed-forward Artificial Neural Network consisting of multiple dense layers. The network takes preprocessed customer features as input and passes them through hidden layers using the ReLU activation function.

The final output layer uses a **sigmoid activation function**, which produces a probability between 0 and 1. This makes the model suitable for binary classification.

The general architecture is:

```text
Input Features
      ↓
Dense Layer (64 neurons, ReLU)
      ↓
Dense Layer (32 neurons, ReLU)
      ↓
Output Layer (1 neuron, Sigmoid)
      ↓
Churn Prediction
```

The model is trained using **binary cross-entropy loss**, which is appropriate for binary classification problems.

## Project Workflow

The complete workflow of the project includes:

```text
Customer Dataset
       ↓
Data Collection
       ↓
Data Cleaning & Preprocessing
       ↓
Feature Transformation
       ↓
Train-Test Split
       ↓
ANN Model Creation
       ↓
Model Training
       ↓
Model Evaluation
       ↓
Model Saving
       ↓
Streamlit Application
       ↓
Customer Churn Prediction
```

## Streamlit Application

The trained ANN model is integrated into a Streamlit web application. Users can provide the required customer information through the application interface, and the model processes the input to generate a churn prediction.

The application is designed to provide an easy-to-use interface where users do not need to write Python code or interact directly with the trained neural network.

The application can predict whether a customer is likely to:

* **Stay with the company**
* **Churn / Leave the company**

This makes the project more practical by connecting the machine learning model with a user-friendly web interface.

## Deployment

The application is deployed using **Streamlit Community Cloud** and the source code is maintained in a GitHub repository.

During deployment, the Python and TensorFlow versions need to be compatible. The project uses TensorFlow for the ANN model, so the deployment environment must use a Python version supported by the selected TensorFlow release.

For example, a compatible setup can use:

```text
Python 3.11
TensorFlow 2.17.0
Streamlit
```

This ensures that the required TensorFlow package can be installed successfully during deployment.

## Business Impact

A customer churn prediction system can help businesses move from a reactive approach to a proactive customer retention strategy.

By identifying customers who have a high probability of leaving, businesses can:

* Identify high-risk customers.
* Improve customer retention.
* Provide personalized offers.
* Reduce customer acquisition and replacement costs.
* Improve customer satisfaction.
* Support data-driven business decisions.

## Future Improvements

The project can be further improved by:

* Hyperparameter tuning of the ANN architecture.
* Comparing ANN performance with models such as XGBoost, Random Forest, and LightGBM.
* Using advanced techniques to handle class imbalance.
* Adding model explainability using SHAP or LIME.
* Improving the Streamlit user interface.
* Adding real-time prediction probability and visualizations.
* Monitoring model performance after deployment.
* Implementing automated model retraining with new customer data.

## Conclusion

This project demonstrates the complete machine learning lifecycle, from data preprocessing and ANN model development to web application deployment. It combines **deep learning, data science, and application deployment** to solve a practical business problem.

The final system provides a simple interface for predicting customer churn and demonstrates how machine learning can be used to support customer retention and business decision-making.
