
# House Price Prediction

## Project Overview

This project focuses on predicting house prices using machine learning techniques. The dataset contains information about residential properties such as number of bedrooms, house type, location, area, area type, and price per square foot.

The project includes data preprocessing, exploratory data analysis, feature preparation, machine learning model training, model evaluation, and house price prediction.

## Objectives

* Clean and preprocess the house price dataset.
* Perform exploratory data analysis to understand price patterns.
* Analyze the relationship between house prices, area, and number of bedrooms.
* Prepare numerical and categorical features for machine learning.
* Train regression models for house price prediction.
* Compare model performance using evaluation metrics.
* Predict the price of a new house based on its features.

## Dataset

The dataset contains **3,968 records and 15 original attributes** related to residential properties.

Important attributes include:

* `Flat_Price` – Price of the property.
* `BHK` – Number of bedrooms.
* `HOUSE_TYPE` – Type of house.
* `Location` – Location of the property.
* `Area_Type` – Type of area measurement.
* `Total_Sq.ft` – Total area of the property.
* `Price_per_sq.ft` – Price per square foot.
* `Owner_type` – Type of property owner.

The target variable for prediction is:

`Flat_Price`

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook

## Project Workflow

### 1. Data Loading

The house price dataset is loaded using Pandas and its structure, dimensions, data types, and missing values are examined.

### 2. Data Preprocessing

The dataset is cleaned by:

* Removing unnecessary columns.
* Handling missing values.
* Converting BHK values into numerical format.
* Converting area values into numerical values.
* Converting price-related values into a standardized numerical format.
* Preparing categorical features for machine learning.

### 3. Exploratory Data Analysis

The following visualizations are used:

* Distribution of house prices.
* House price distribution by BHK.
* House price versus total area.
* Correlation heatmap.

### 4. Feature Preparation

Numerical and categorical features are separated. Categorical variables are encoded using One-Hot Encoding.

A preprocessing pipeline is used to ensure that the same transformations are applied to both training and testing data.

### 5. Machine Learning Models

The following regression algorithms are implemented:

* Linear Regression
* Random Forest Regression

### 6. Model Evaluation

The models are evaluated using:

* Mean Absolute Error (MAE)
* Root Mean Squared Error (RMSE)
* R² Score

The model performance is compared to identify the better-performing regression model.

### 7. Prediction

The trained model is used to predict the price of a new house using property details such as BHK, location, house type, area, and owner type.

## Project Structure

```text
DataAnalytics-L2-HousePricePrediction/
│
├── House_Price_Prediction.ipynb
├── house_price_dataset.csv
├── README.md
│
└── screenshots/
    ├── price_distribution.png
    ├── price_by_bhk.png
    ├── area_vs_price.png
    ├── correlation_heatmap.png
    ├── actual_vs_predicted.png
    └── model_comparison.png
```

## Results

The project compares Linear Regression and Random Forest Regression based on MAE, RMSE, and R² Score.

The **Actual vs Predicted** visualization is used to examine how closely the predicted house prices match the actual prices.

## Conclusion

This project demonstrates the complete machine learning workflow for house price prediction, starting from raw data preprocessing and exploratory analysis to model training, evaluation, and prediction.

The project provides practical experience in regression, feature preprocessing, categorical encoding, model comparison, and data visualization.

## Author

**Jahnavi Naik**

Data Analytics Project
Oasis Infobyte Internship Program
