# PRODIGY_ML_01
## House Price Prediction Using Linear Regression
### 1- Project Overview
This project contains implementation and evaluation of a linear regression model to predict house prices based on three key features: square footage (GrLivArea), number of bedrooms (BedroomAbvGr), and number of full bathrooms (FullBath). The dataset used in this project is derived from the House Prices: Advanced Regression Techniques competition on Kaggle.

The objective of this project is to develop a regression model that can estimate house prices based on the selected features and evaluate the model's performance using appropriate metrics.

### 2- Dataset Description
The dataset consists of two files:
- **train.csv:** This dataset includes 1460 rows of house sales data with 81 features, including the target variable SalePrice.
- **test.csv:** This dataset contains 1459 rows without the SalePrice, which is to be predicted using the trained model.

**Key Features Used in the Model**:
- **GrLivArea: Above grade living area in square feet.**
- **BedroomAbvGr: Number of bedrooms above ground.**
- **FullBath: Number of full bathrooms.**
- **SalePrice: The sale price of the house (target variable).**

**Dataset Exploration**
To understand the dataset, the following steps were taken:

- **Data Inspection: The first few rows of both the training and test datasets were displayed to understand the structure.**
- **Dataset Statistics: Summary statistics (mean, standard deviation, min, max) were computed for the key features.**
- **Missing Data: Missing values were identified and handled by dropping rows with missing values in the selected features.**
- **Duplicated Data: Checked for any duplicate rows and removed them if found.**


### 3- Data Preprocessing
Preprocessing is essential for preparing the data for the model. The following steps were taken:

- **Feature Selection: Three features (GrLivArea, BedroomAbvGr, and FullBath) were selected for training the model as they are directly related to housing characteristics and are likely to influence the sale price.**
- **Handling Missing Values: Rows with missing values in the selected features were dropped.**
- **Data Splitting: The dataset was split into training and validation sets, with 80% of the data used for training and 20% reserved for validation. This ensures that the model is evaluated on unseen data.**



### 4- Model Description
The machine learning model chosen for this project is Linear Regression, a widely-used algorithm for regression tasks that models the relationship between one dependent variable and one or more independent variables.
**Why Linear Regression?** :
Linear regression is ideal for this task because it is a simple yet effective algorithm for predicting continuous values, such as house prices, based on the relationship between the input features.

**Libraries Used**
- **pandas: For data manipulation and loading the datasets.**
- **scikit-learn: To split the dataset, train the linear regression model, and calculate performance metrics.**
- **LinearRegression: The model used to predict house prices.**
- **train_test_split: To split the dataset into training and validation sets.**
- **mean_squared_error, r2_score, mean_absolute_error: For performance evaluation.**
- **matplotlib: For visualizing the results.**


### 5- Model Training and Evaluation
**Training** :
- **Linear Regression Model: The model was trained using the LinearRegression class from the scikit-learn library.**
- **The input features were GrLivArea, BedroomAbvGr, and FullBath. The target variable was SalePrice.**


** Evaluation Metrics**:
After training the model, several evaluation metrics were calculated to assess its performance:

- **Mean Squared Error (MSE): Measures the average squared difference between actual and predicted values. Lower values are better.**
- **R² Score: Indicates the proportion of variance in the target variable explained by the model. A higher R² score indicates a better fit.**
- **Mean Absolute Error (MAE): Represents the average magnitude of errors in the predictions, without considering their direction.**



#### Finally :


This project implemented a simple yet effective linear regression model to predict house prices based on square footage, number of bedrooms, and number of bathrooms. While the model achieved a reasonable performance with an R² of 0.63 and an MAE of approximately $35,788, there is room for improvement by:

- **Incorporating additional features (e.g., location, year built, etc.)**
- **Experimenting with more advanced models such as decision trees, random forests, or gradient boosting.**
- **Fine-tuning hyperparameters.**
Overall, this project demonstrates the power of linear regression for predictive modeling in real estate and offers opportunities for further exploration.
