# Housing Price Prediction with Linear Regression

This project implements simple and multiple linear regression models to predict house prices using the Housing.csv dataset. The dataset includes key house features such as area, number of bedrooms, bathrooms, stories, and various amenities, enabling accurate price predictions through regression analysis.

## Objectives

- Develop a simple linear regression model using the area feature to predict house prices.
- Build a multiple linear regression model incorporating all available features.
- Preprocess the dataset by handling categorical variables through binary mapping and one-hot encoding.
- Evaluate model performance using Mean Absolute Error (MAE), Mean Squared Error (MSE), and R² score.
- Visualize results with:
  - A scatter plot of actual vs. predicted prices for multiple linear regression.
  - A regression line plot for simple linear regression (Price vs. Area).

## Dataset

The dataset (Housing.csv) includes the following columns:

- **price**: House price (target variable, in monetary units).
- **area**: House area in square feet.
- **bedrooms**: Number of bedrooms.
- **bathrooms**: Number of bathrooms.
- **stories**: Number of stories.
- **mainroad**: Connection to the main road (yes/no).
- **guestroom**: Presence of a guest room (yes/no).
- **basement**: Presence of a basement (yes/no).
- **hotwaterheating**: Presence of hot water heating (yes/no).
- **airconditioning**: Presence of air conditioning (yes/no).
- **parking**: Number of parking spaces.
- **prefarea**: Location in a preferred area (yes/no).
- **furnishingstatus**: Furnishing status (furnished, semi-furnished, unfurnished).

## Requirements

Ensure the following Python libraries are installed:
install pandas numpy scikit-learn matplotlib

Project Structure
housing_linear_regression.py: Main script implementing data preprocessing, model training, evaluation, and visualization.
Housing.csv: Dataset used for training and testing the regression models.
simple_linear_regression.png: Output plot showing price vs. area with the fitted regression line.
multiple_linear_regression.png: Output plot comparing actual vs. predicted prices for multiple linear regression.
README.md: This file, providing project details and instructions.
Setup and Execution
Clone or download this repository:

Copy
git clone https://github.com/yourusername/yourproject.git
cd yourproject
Place Housing.csv in the same directory as housing_linear_regression.py.

Install the required libraries (see Requirements).

Run the script:

Copy
python housing_linear_regression.py
The script will:
Load and preprocess the dataset, converting categorical variables (yes/no) to binary (1/0) and one-hot encoding furnishingstatus.
Split data into 80% training and 20% testing sets with a fixed random seed (random_state=42).
Train and evaluate simple and multiple linear regression models.
Print performance metrics (MAE, MSE, R²) and model coefficients.
Generate and save two plots: simple_linear_regression.png and multiple_linear_regression.png.
Outputs
Console Output
Displays MAE, MSE, R² scores, coefficients, and intercepts for both models. Example (values vary based on data split):

Simple Linear Regression (using area):

MAE: 1234567.89
MSE: 2345678901234.56
R²: 0.45
Coefficient (area): 456.78
Intercept: 1234567.89
Multiple Linear Regression:

MAE: 987654.32
MSE: 1234567890123.45
R²: 0.68
Coefficients:
area: 345.67
bedrooms: 234567.89
...
Intercept: 987654.32
Visualizations
simple_linear_regression.png: Scatter plot of house prices vs. area with the regression line.
multiple_linear_regression.png: Scatter plot of actual vs. predicted prices for multiple linear regression.
Model Interpretation
Simple Linear Regression: The area coefficient indicates the price change per square foot increase.
Multiple Linear Regression: Each feature’s coefficient reflects the price change per unit increase, holding other features constant. Positive coefficients increase prices, while negative ones decrease them.
Notes
Preprocessing: Binary variables are mapped to 1/0, and furnishingstatus is one-hot encoded for model compatibility.
Data Split: An 80/20 train-test split ensures robust evaluation, with a fixed random seed for reproducibility.
Model Scope: Simple regression uses only area, while multiple regression leverages all features for improved accuracy.
Future Enhancements
Apply feature selection to identify high-impact predictors.
Experiment with advanced regression techniques (e.g., Ridge, Lasso).
Implement feature scaling or outlier removal for enhanced performance.
Use k-fold cross-validation for more reliable evaluation.
