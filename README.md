# Pyspark Machine Learning House Price Prediction

## Kaggle Competition selected
This is a competition to predict house prices using advanced regression techniques. It is aimed at beginner data science students who have experience with some R or Python and machine learning basics. The goal is the predict the sales price for each house in the test set. Here is the link for the project: https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/overview

## Data exploration

Sales price vs Log of Sale Price


![image](https://user-images.githubusercontent.com/78801723/169141940-de6bf62c-e996-42e8-976f-a4dabaee3b2b.png)


![image](https://user-images.githubusercontent.com/78801723/169141957-482188b5-f4c1-4eae-b090-256e88843683.png)

Correlation Matrix


![image](https://user-images.githubusercontent.com/78801723/169142062-32fe2681-be2e-4b00-8836-0ac6ad9fdd2b.png)

Description of top 9 correlated values
- OverallQual: Rates the overall material and finish of the house (1 = Very Poor, 10 = Very Excellent)
- GrLivArea: Above grade (ground) living area square feet
- GarageCars: Size of garage in car capacity
- GarageArea: Size of garage in square feet
- TotalBsmtSF: Total square feet of the basement area
- 1stFlrSF: First Floor square feet
- FullBath: Full bathrooms above grade
- TotRmsAbvGrd: Total rooms above grade (does not include bathrooms)
- YearBuilt: Original construction date

![image](https://user-images.githubusercontent.com/78801723/169142251-08d4e947-4313-4bee-a1e3-f4d76cb7a334.png)
![image](https://user-images.githubusercontent.com/78801723/169142261-3483c2e6-9e0b-4c59-baba-9d0e5247f513.png)
![image](https://user-images.githubusercontent.com/78801723/169142278-ccf3bcf8-8186-4984-a447-7f433f08fa2c.png)
![image](https://user-images.githubusercontent.com/78801723/169142286-3fd31889-109d-45e0-926a-e3b411cd864d.png)
![image](https://user-images.githubusercontent.com/78801723/169142320-5f50cd55-4fc9-4261-b622-d9db512cba3d.png)
![image](https://user-images.githubusercontent.com/78801723/169142336-ca85b2f6-7cec-488e-9435-77682eb561c6.png)
![image](https://user-images.githubusercontent.com/78801723/169142357-ecb19014-20f5-45f0-b2f5-869af9c02520.png)

### Models and results

1. LinearRegression


![image](https://user-images.githubusercontent.com/78801723/169142502-6581cc28-6e02-4fec-a2c7-8a478d9564b3.png)

2. RandomForestRegressor


![image](https://user-images.githubusercontent.com/78801723/169142583-9f8f6987-5b95-4f56-a67c-d78ce962fd98.png)

3. DecisionTreeRegressor


![image](https://user-images.githubusercontent.com/78801723/169142624-a3baebc1-9d0c-4cd7-9c5a-a70b19cefc26.png)

