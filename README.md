# 🏠 House Price Prediction System

## 📌 Project Overview

The **House Price Prediction System** is a Machine Learning application that predicts residential property prices based on different property features such as location, area, number of bedrooms, number of bathrooms, property age, parking spaces, and floor number.

The project implements a complete Machine Learning workflow, including data cleaning, exploratory data analysis, preprocessing, feature engineering, regression model development, model evaluation, and a prediction interface.

---

## 🎯 Objectives

The main objectives of this project are:

- To clean and preprocess housing data.
- To perform Exploratory Data Analysis (EDA).
- To perform feature engineering and categorical encoding.
- To develop a regression model for house price prediction.
- To evaluate the performance of the Machine Learning model.
- To provide an interactive prediction interface.
- To save the trained Machine Learning model for future predictions.

---

## ✨ Key Features

- ✅ Data Cleaning & Preprocessing
- ✅ Exploratory Data Analysis (EDA)
- ✅ Feature Engineering
- ✅ One-Hot Encoding
- ✅ Random Forest Regression
- ✅ Model Performance Evaluation
- ✅ Actual vs Predicted Visualization
- ✅ Trained Model Saving
- ✅ Interactive Prediction Interface

---

## 🛠️ Technologies Used

- **Python**
- **Pandas**
- **NumPy**
- **Scikit-learn**
- **Matplotlib**
- **Joblib**
- **Jupyter Notebook**
- **GitHub**

---

## 🤖 Machine Learning Algorithm

The project uses the:

### Random Forest Regressor

Random Forest is an ensemble Machine Learning algorithm that combines multiple decision trees to make predictions.

It was selected because it can effectively handle:

- Non-linear relationships
- Multiple input features
- Feature interactions
- Numerical and categorical data after preprocessing

---

## 📊 Dataset

The project contains a synthetic housing dataset with **500 property records**.

### Dataset Features

| Feature | Description |
|---|---|
| `location` | Location/city of the property |
| `area_sqft` | Property area in square feet |
| `bedrooms` | Number of bedrooms |
| `bathrooms` | Number of bathrooms |
| `age_years` | Age of the property |
| `parking_spaces` | Number of parking spaces |
| `floor` | Floor number |
| `price_inr` | Property price in Indian Rupees |

### Example Data

```text
location,area_sqft,bedrooms,bathrooms,age_years,parking_spaces,floor,price_inr
Chennai,1500,3,2,5,1,4,XXXXX
Bangalore,2200,4,3,3,2,6,XXXXX
Hyderabad,1200,2,2,8,1,2,XXXXX
