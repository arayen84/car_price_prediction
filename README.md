# car_price_prediction
This project combines elements of data cleaning, data analysis, data visualization, and machine learning. It demonstrates a typical workflow for developing a predictive model for car prices using linear regression and lasso regression techniques.

## Car Price prediction Machine Learning Model

### Dataset Features
* Car brand
* Year
* Sold Price
* Present Price
* KMS Driven
* Fuel Type
* Seller Type
* Transmission Type
* Owners

### Worlflow 
Dataset ---> Data Preprocessing ---> Train Test Split ---> Linear & Lasso Regression Model 


New Data ---> Trained Linear & Lasso Regression Model ---> Predicted car price

### Dataset 
https://www.kaggle.com/datasets/nehalbirla/vehicle-dataset-from-cardekho

### Data Loading 

Project started by importing the necessary libraries and loading the dataset from a CSV file into a Pandas DataFrame using pd.read_csv('/content/car data.csv').

### Data Cleaning

car_dataset.info(): 

This command provides information about the dataset, including data types and non-null counts, which is useful for understanding the dataset's structure.

car_dataset.isnull().sum(): 
It checks for missing values in the dataset, which is an essential part of data cleaning. In this case, it appears that there are no missing values.

car_dataset.replace(...): 

This code snippet is used to encode categorical variables like "Fuel_Type," "Seller_Type," and "Transmission" into numerical values. This is often done to prepare the data for machine learning models since many algorithms require numerical inputs.

### Data Mining

discovering patterns of the dataset and preparing the data for machine learning.

### Data Analysis

Exploring the dataset's characteristics, such as the distribution of categorical data (Fuel_Type, Seller_Type, Transmission) using value_counts(), is a form of data analysis. Understanding the distribution of variables can help in feature selection and model building decisions.

### Data Visualization

You create scatter plots to visualize the relationships between actual prices and predicted prices for both the training and testing data sets. These scatter plots are used to assess the performance of your regression models visually. Visualization is a crucial step in understanding the model's behavior.

### Machine Learning Model Building and Evaluation:

Split the dataset into training and testing sets using train_test_split().
Build two regression models: Linear Regression and Lasso Regression.
Fit the models to the training data and make predictions on both the training and testing data.
Calculate the R-squared error (metrics.r2_score()) to evaluate the model's performance. R-squared measures how well the model fits the data.
Use scatter plots to visualize the relationship between actual and predicted values, which is an essential part of model evaluation.
