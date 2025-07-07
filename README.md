Housing Price Prediction with Linear Regression

Project Overview

This project implements both simple and multiple linear regression models to predict house prices based on the Housing.csv dataset. The dataset contains various features of houses such as area, number of bedrooms, bathrooms, stories, and other amenities, which are used to predict the price of a house.

Objectives





Implement simple linear regression using the area feature to predict house prices.



Implement multiple linear regression using all available features.



Preprocess the dataset, including handling categorical variables.



Evaluate model performance using Mean Absolute Error (MAE), Mean Squared Error (MSE), and R² score.



Visualize results with scatter plots for actual vs. predicted prices and regression lines.

Dataset

The dataset (Housing.csv) contains the following columns:





price: The price of the house (target variable).



area: Area of the house in square feet.



bedrooms: Number of bedrooms.



bathrooms: Number of bathrooms.



stories: Number of stories.



mainroad: Whether the house is connected to the main road (yes/no).



guestroom: Whether the house has a guest room (yes/no).



basement: Whether the house has a basement (yes/no).



hotwaterheating: Whether the house has hot water heating (yes/no).



airconditioning: Whether the house has air conditioning (yes/no).



parking: Number of parking spaces.



prefarea: Whether the house is in a preferred area (yes/no).



furnishingstatus: Furnishing status (furnished, semi-furnished, unfurnished).

Requirements

To run the code, you need the following Python libraries:





pandas



numpy



scikit-learn



matplotlib

You can install these dependencies using pip:

pip install pandas numpy scikit-learn matplotlib

File Structure





housing_linear_regression.py: The main Python script containing the implementation of linear regression models.



Housing.csv: The dataset used for training and testing the models.



simple_linear_regression.png: Output plot for simple linear regression (Price vs. Area).



multiple_linear_regression.png: Output plot for multiple linear regression (Actual vs. Predicted Prices).



README.md: This file, providing an overview of the project.

How to Run





Ensure you have the required libraries installed.



Place the Housing.csv dataset in the same directory as the housing_linear_regression.py script.



Run the script using Python:

python housing_linear_regression.py



The script will:





Load and preprocess the dataset.



Train and evaluate both simple and multiple linear regression models.



Print performance metrics (MAE, MSE, R²) and model coefficients.



Generate and save two plots: simple_linear_regression.png and multiple_linear_regression.png.

Output





Console Output: The script prints the MAE, MSE, and R² scores for both models, along with the coefficients and intercepts for interpretation.



Plots:





simple_linear_regression.png: A scatter plot of house prices vs. area with the fitted regression line.



multiple_linear_regression.png: A scatter plot of actual vs. predicted prices for the multiple linear regression model.



Model Interpretation:





For simple linear regression, the coefficient indicates the price change per unit increase in area.



For multiple linear regression, each coefficient shows the price change per unit increase in the respective feature, holding others constant.

