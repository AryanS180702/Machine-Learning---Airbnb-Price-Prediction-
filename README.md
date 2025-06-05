# Airbnb Price Prediction

## Dataset
The dataset used in this project is Airbnb listing data, where the target variable is `log_price`.  
Input variables include:
- **Categorical features**: `property_type`, `room_type`, `city`, `bed_type`, etc.  
- **Numerical features**: `number_of_bathrooms`, `number_of_bedrooms`, `number_of_beds`, `accommodates`, etc.

🔗 [Airbnb Price Dataset](https://docs.google.com/spreadsheets/d/1N7P0euUjfjB8XXdTBQeicjGjxAOm18wvCRLaQC92a8g/edit?usp=sharing) 


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
