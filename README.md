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

## 📂 Files
- `Housing.csv` (Original dataset)
- `implementation.ipynb` (Jupyter Notebook with code)
- `README.md` (This documentation)

## 🚀 How to Use
1. Clone the repo:
   ```bash
   git clone https://github.com/satwikkajjam/implementation.git

## 📊 Visualization
- simple_linear_regression.png: Scatter plot of house prices vs. area with the regression line.
- multiple_linear_regression.png: Scatter plot of actual vs. predicted prices for multiple linear regression.

