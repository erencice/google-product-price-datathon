# 🏷️ Datathon 2025 – Google AI Academy

## 📑 Table of Contents
- [Problem Definition](#problem-definition)  
- [Data Files](#data-files)  
- [Data Features](#data-features)  
- [Data Exploration & Preprocessing](#data-exploration--preprocessing)  
- [Data Analysis & Visualization](#data-analysis--visualization)  
- [Modeling & Evaluation](#modeling--evaluation)  
- [Key Features](#key-features)  

---

## 🧩 Problem Definition

This project was developed as part of the **Datathon 2024**, mainly organized by **Google AI Academy**
The competition aimed to provide participants with an opportunity to apply their theoretical knowledge in data science to real-world problems.  
Participants worked on analyzing large datasets to extract meaningful insights and develop predictive models. 

Product prices vary depending on their characteristics, category, production location, the market where they are sold, and the city. The goal is to predict product prices based on the provided training data and to achieve accurate predictions for the test data.

The primary objective was to predict product prices based on various features, including product characteristics, category, production location, market type, and city.

---

## **📂 Data Files**
- **train.csv:** Training dataset containing product features and prices.  
- **testFeatures.csv:** Test dataset containing product features for which price predictions are expected.  
- **sample_submission.csv:** Sample submission file showing the required format to submit predictions for all products in the test set.

---

## **Data Contents:**  
For each product in the training and test datasets, the following information is provided:  
- **Date:** The date when product features were recorded.  
- **Product Name:** The name of the product.  
- **Product Nutritional Value:** The nutritional value of the product.  
- **Product Category:** The category to which the product belongs.  
- **Product Price:** The price of the product (available only in the training set).  
- **Production Location:** The place where the product was produced.  
- **Market:** The market where the product is sold.  
- **City:** The city where the product is sold.

**Objective:** This project aims to predict product prices for the test dataset and maximize the accuracy of these predictions.

---

## 🧹 Data Exploration & Preprocessing

- **Training data**: 227,520 observations, 8 features  
- **Test data**: 45,504 observations, 8 features  
- **Libraries used**: `pandas`, `numpy`, `seaborn`, `matplotlib`, `lightgbm`, `optuna`  
- **Steps performed**:
  - Missing value analysis  
  - Outlier detection and treatment  

---

## 📊 Data Analysis & Visualization

Key visualizations include:

- Average price by **product category** and **city**  
- Distribution analysis via **pie charts** and **histograms**  
- Correlation analysis between numerical features  
- Relationship between **nutritional value** and **price**  
- Price distribution segmented by **city** and **market type**  

---

## ⚙️ Modeling & Evaluation

- **Categorical variables** transformed using **dummy variables**  
- Implemented **LightGBM** model  
- Used **Optuna** for hyperparameter tuning  
- Analyzed **feature importance**  
- Adjusted predictions using a **monthly price increase rate of 1.05%**  
- Generated final predictions in required submission format  

---

## 🌟 Key Features

The model identified the **top 10 most important features** affecting product price. These were visualized with feature importance plots to interpret the model's behavior and reasoning.
