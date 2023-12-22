# OIBSIP-5

SALES PREDICTION USING PYTHON

Sales prediction means predicting how much of a product people will buy based on factors
such as the amount you spend to advertise your product, the segment of people you
advertise for, or the platform you are advertising on about your product.

Typically, a product and service-based business always need their Data Scientist to predict
their future sales with every step they take to manipulate the cost of advertising their
product. So let’s start the task of sales prediction with machine learning using Python.

Explaination: 
1. Data Loading and Exploration (EDA):
- Reads a dataset from a CSV file using pandas.
- Conducts exploratory data analysis (EDA) by displaying the first and last few rows, summary statistics, information about the dataset, checking for missing values, and checking for duplicated rows.
- Renames the 'Unnamed: 0' column to 'Index' for clarity.
- Plots histograms for each feature and a pair plot to visualize relationships between features and the target variable 'Sales'.
- Displays boxplots to identify outliers.

2. Correlation Analysis:
- Calculates and displays the correlation matrix using df.corr().
- Visualizes the correlation matrix using a heatmap.

3. Data Preprocessing:
- Defines the features 'X' (TV, Radio, Newspaper) and the target variable 'Y' (Sales).
- Splits the dataset into training and testing sets using train_test_split.
- Initializes a StandardScaler and scales the training and testing features.

4. Linear Regression Model:
- Initializes a linear regression model (model1).
- Trains the model on the scaled training data.
- Makes predictions on the scaled test data.
- Evaluates the model using mean squared error (MSE) and R-squared.
- Visualizes the predictions vs. actual values using a scatter plot.

5.Decision Tree Model:
- Initializes a decision tree regressor model (model2).
- Trains the model on the original (unscaled) training data.
- Makes predictions on the original test data.
- Evaluates the model using mean squared error (MSE) and R-squared.
- Visualizes the decision tree using tree.plot_tree.

6.User Input and Prediction:
- Takes user input for new data (TV, Radio, Newspaper values).
- Creates a DataFrame for the new data.
- Scales the new data using the same scaler used for the linear regression model (model1).
- Predicts sales for the new data using both the linear regression model (model1) and the decision tree model (model2).
- Prints the predicted sales for the new data.
  
