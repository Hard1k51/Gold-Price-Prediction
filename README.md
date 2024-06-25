# Gold-Price-Prediction
This project focuses on predicting the price of gold using historical data and machine learning techniques. The goal is to provide accurate predictions that can assist in financial decision-making. The dataset spans from 2008 to 2018, providing a comprehensive view of the factors influencing gold prices over a decade.

#Dataset
The dataset used for this project is gld_price_data.csv, which contains the following columns:

Date: The date of the recorded data point.
GLD: The price of gold on that particular date.
Additional columns representing various financial indicators and metrics that could influence gold prices.

#Key Steps and Methodology
1)Data Loading and Exploration

Loaded the dataset using pandas.
Explored the first few and last few rows using df.head() and df.tail().
Described the dataset to understand the basic statistics using df.describe().
Checked the data types of each column using df.dtypes.

2)Data Preprocessing
Converted the Date column to datetime format.
Selected only numeric columns for correlation analysis.
Computed and visualized the correlation matrix using seaborn.heatmap().

3)Feature Selection and Splitting
Dropped the Date and GLD columns to create feature set X.
Set GLD as the target variable Y.
Split the data into training and testing sets using train_test_split from sklearn.

4)Model Training
Used a RandomForestRegressor with 100 estimators to train the model.
Evaluated the model performance using R-squared error.

5)Model Evaluation
Predicted gold prices on the test set.
Visualized the real vs. predicted values using matplotlib.
Computed evaluation metrics: Mean Absolute Error (MAE), Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and R-squared error.
Calculated the model accuracy percentage.


#Results
R-squared Error: Indicates how well the model's predictions match the actual values.
Mean Absolute Error (MAE): Measures the average magnitude of errors in the predictions.
Mean Squared Error (MSE) and Root Mean Squared Error (RMSE): Provide insights into the variance of the prediction errors.
Model Accuracy: The percentage of variation explained by the model.


#Visualization
Correlation Heatmap: Displays the correlation between different features and the target variable (GLD).
Distribution Plot: Shows the distribution of the gold prices.
Real vs. Predicted Prices Plot: Compares the actual gold prices with the predicted values to visually assess the model's performance.


#Dependencies
pandas
numpy
matplotlib
seaborn
sklearn
