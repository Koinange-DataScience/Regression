Exercise 1:
-The average temperature and solar panel output data are converted into NumPy arrays for easy manipulation
-plt.scatter creates a scatter plot with average temperature on the X-axis and solar panel output on the Y-axis
-plt.xlabel and plt.ylabel label the axes, while plt.title adds a title to the plot
-plt.show() displays the plot. 

Findings
-There is not a linear relationship between the average temperature of a day and the energy produced by solar panels. 
-Maybe other factors that we havent accounted for could be the cause
-This means that a linear regression mode will not be a good fit for our data


Exercise 2:
-The code converts the lists of annual_rainfall and agricultural_yield into NumPy arrays for compatibility with sklearn's Linear Regression model. The reshape(-1, 1) is applied to annual rainfall to convert it from a 1D to a 2D array because sklearn expects X (features) to be a 2D array
-A LinearRegression model is instantiated and fitted to the data with .fit(), modelling the relationship between rainfall and yield 
-.predict() is used to estimate the yield for a specific value of rainfall(1150mm), demonstrating how the model can be used to make predictions based on new input data
-The predicted yield is printed, providing actionable insights based on the model

Exercise 3:
-The code first fits a Linear regression model to the traffic volume and pollution level data
-After fitting the model, it uses the model to predict pollution levels based on the observed traffic volumes. 
-It calculates the mean squared error (MSE) and R-squared value using sklearn's mean_squared_error and r2_score functions
