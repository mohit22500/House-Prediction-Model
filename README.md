# House_Price_Prediction_Model
This project is a machine learning model aimed at predicting house prices based on several features such as carpet area, number of floors, ownership, and more. The dataset has been processed, and multiple regression models have been applied to predict the house prices accurately.

# Introduction
The goal of this project is to predict the price of houses based on a dataset containing various attributes of the house. The project performs data preprocessing, feature engineering, and trains multiple machine learning models to predict house prices. The models include:

- Random Forest Regressor
- Gradient Boosting Regressor
- XGBoost Regressor

# Dataset
The dataset used for this project is assumed to be stored in a CSV file named house_prices.csv. It contains various attributes such as:

- Carpet Area
- Price
- Ownership
- Location
- Floor Information
- Bathroom, Balcony count, etc.

# Required Libraries:
- NumPy
- pandas
- seaborn
- matplotlib
- scikit-learn
- XGBoost

# Data Preprocessing
Steps involved in preprocessing:
1. Null Value Handling: Columns with more than 50% null values are dropped. Remaining null values are imputed using mode (for categorical data) or mean (for numerical data).
2. Data Type Conversion:
  - Carpet Area data is converted from strings like "sqft" or "sqm" to numerical values.
  - Amount is converted from formats like "Lac" and "Cr" to a float representing the actual value in rupees.
3. Categorical Encoding: Categorical features such as 'Transaction', 'Location', 'Furnishing', etc., are label encoded.
4. Feature Engineering:
  - The 'Floor' column is split into two columns, current_floor and total_floors.
  - Columns like 'Bathroom' and 'Balcony' with values greater than 10 are capped at 11.
5. Standardization: Features such as 'Price in Rupees' and 'Carpet Area' are standardized for better performance in regression models.

# Model Training
The following machine learning models were trained:

- Random Forest Regressor
- Gradient Boosting Regressor
- XGBoost Regressor

# Model Training Process:
- The dataset was split into 70% training and 30% testing.
- Each model was trained on the training data and evaluated using the test data.
- Metrics such as R-squared, Mean Absolute Error (MAE), and Root Mean Squared Error (RMSE) were used to evaluate the models.

# Evaluation Metrics
After training the models, their performance was evaluated using the following metrics:
- R-Squared: A statistical measure representing the proportion of variance for the dependent variable explained by the independent variables.
- Mean Absolute Error (MAE): The average magnitude of the errors between predicted and actual values.
- Root Mean Squared Error (RMSE): The square root of the average squared differences between predicted and actual values.
- Model Accuracy: Percentage of correct predictions.


