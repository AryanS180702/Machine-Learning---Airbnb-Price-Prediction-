# Machine-Learning---Airbnb-Price-Prediction-

# Airbnb Price Prediction

## Overview
Airbnb provides a platform for property owners to rent out their spaces to travelers. Pricing a listing effectively is critical for maximizing revenue while staying competitive in the market. For hosts, understanding what factors influence the price of their listings is essential. This project aims to build a machine learning model to predict the price of Airbnb listings based on various features such as property type, room type, location, amenities, and host characteristics. By analyzing these factors, this project provides actionable insights to Airbnb hosts to help optimize their listing prices.

## Problem Statement
The main objective of this project is to develop a regression model that can predict the price of an Airbnb listing. Using features like property type, number of reviews, location, and available amenities, the model aims to estimate the listing price with reasonable accuracy. The insights from this project can help Airbnb hosts understand what drives pricing, enabling them to make data-informed decisions. It can also help Airbnb improve its pricing recommendations to enhance user satisfaction on both ends.

## Dataset
The dataset used in this project is Airbnb listing data, where the target variable is `log_price`.  
Input variables include:
- **Categorical features**: `property_type`, `room_type`, `city`, `bed_type`, etc.  
- **Numerical features**: `number_of_bathrooms`, `number_of_bedrooms`, `number_of_beds`, `accommodates`, etc.

## Approach

1. **Data Import**  
   - Loaded the Airbnb dataset into a pandas DataFrame.

2. **Data Cleaning**  
   - Identified and handled missing values  
   - Dropped irrelevant or redundant columns

3. **Feature Engineering**  
   - Created new features from existing ones  
   - Visualized new variables and their relationship with the target (`log_price`)

4. **Exploratory Data Analysis (EDA)**  
   - Analyzed the distribution of the target variable  
   - Studied categorical features and their frequency  
   - Explored correlations between numerical features using pairplots and heatmaps

5. **Data Transformation**  
   - Applied encoding techniques to handle categorical variables

6. **Model Development and Evaluation**  
   - Split data into training and testing sets  
   - Scaled numerical features  
   - Trained a Ridge Regression model  
   - Performed hyperparameter tuning and cross-validation to improve performance and reduce overfitting

7. **Prediction Class**  
   - Built a custom prediction class that takes input features and returns the predicted price

## Results
The Ridge Regression model performed reasonably well in predicting the `log_price` of Airbnb listings. It helped highlight key drivers of price, such as location, property type, and number of amenities.

**Model Performance:**
- R² Score: 0.5573
- Mean Squared Error (MSE): 0.227

## Tools Used
- Python
- pandas, NumPy
- matplotlib, seaborn
- scikit-learn

## Author
Aryan Suresh  
[GitHub Profile](https://github.com/aryansuresh)
