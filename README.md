# Car Price Prediction Model
## Overview
This project aims to build a predictive model that estimates the price of cars in the U.S. market. The model uses various independent variables (such as the car's brand and model) to predict the price of a car. This tool is intended to assist a Chinese automobile company, Geely Auto, which is preparing to enter the U.S. market by understanding pricing dynamics. By leveraging the model, the company can tailor its pricing strategy and make informed decisions regarding car design, production, and market entry.

## Objective
Geely Auto seeks to understand the significant factors affecting car prices in the American market. The model will highlight which variables (such as car company name, car model, etc.) are most influential in predicting car prices. The company can use these insights to adapt their business strategy, enhance competitiveness, and successfully launch in the U.S. market.

- Key Features
Data Preparation: The dataset includes a variable CarName that contains both the car company name and model. For modeling purposes, only the car company name is used as an independent variable.

- Predictive Modeling: Linear regression is used to model the relationship between the car's features and its price.

- Model Evaluation: The model’s performance is evaluated using the R-squared score on the test dataset. The R-squared value helps determine how well the model fits the data.

## Business Impact
By understanding which variables impact car pricing, Geely Auto will have valuable insights for the pricing strategies in the U.S. market. The model’s output can help adjust their designs, features, and pricing based on key market trends and competitor analysis.

## Analysis Process
The project follows a structured analysis process divided into 10 key steps:

1. **Data Sourcing & Understanding**: Understanding the dataset and its features.
   The dataset consists of various features related to car specifications, including attributes such as CarName, fueltype, enginesize, curbweight, and price. These features will help in analyzing the factors that influence car pricing in the U.S. market.

2. **Data Cleaning & Manipulation**: Cleaning the dataset, handling missing values, and preprocessing for model building.
  The dataset contains no missing values, so minimal data cleaning was required. The CarName column, which combines the car company name and model, was split into two separate columns: CompanyName and ModelName. This preprocessing step ensures that only the relevant CompanyName is used as an independent variable for model building.e

3. **Exploratory Data Analysis (EDA)**: Conducting univariate and bivariate analysis to explore relationships between variables.
  Univariate analysis was performed on both numerical and categorical columns to examine the distribution of the data, using histograms for numerical features and boxplots for categorical features. For bivariate analysis, relationships between numerical variables were explored, including their correlation with the target column, price, to identify significant predictors. This helped in understanding how various features influence car prices.
4. **Model Preparation**: Setting up the data for modeling, including feature selection.
First, we check the unique values in all categorical columns to understand their distribution. Then, we convert these categorical columns into numerical values using label encoding. Finally, we apply the linear regression algorithm to the preprocessed data to predict the car prices.
5. **Training & Testing Data Split**: Dividing the dataset into training and testing sets to evaluate the model’s performance.
The dataset is split into training and testing sets using an 80-20 ratio, with 80% for training and 20% for testing. The model is trained on the training data and predictions are made on the test set. The R-squared score is then calculated to assess the model's performance on the test data.
6. **Model Building**: Developing a linear regression model to predict car prices.
 In the simple regression model, enginesize and highwaympg were selected as the two variables to predict car prices. Enginesize reflects the car's engine capacity, while highwaympg represents its fuel efficiency on highways. These variables were chosen to understand how they individually influence car pricing, with enginesize typically expected to have a positive relationship with price, and highwaympg often correlating with price based on fuel efficiency preferences in the market.

## Conclusion
This project provides a predictive tool for understanding car pricing in the U.S. market, helping Geely Auto develop a strategy for entering the market and competing with existing automakers. The analysis and model offer actionable insights for the company to adapt and succeed in the American automotive industry.
