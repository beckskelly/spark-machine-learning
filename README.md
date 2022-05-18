# Pyspark Machine Learning House Price Prediction

This was a project to solve a machine learning problem using pyspark. 

## Kaggle Competition selected
This is a competition to predict house prices using advanced regression techniques. It is aimed at beginner data science students who have experience with
some R or Python and machine learning basics. I picked this project for this reason, as a software development student, I do not have a lot of experience with
machine learning and had to do a lot of background reading for this assignment. The goal is the predict the sales price for each house in the test set. Here is the
link for the project: https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/overview

Problem definition
Task (T): Predict the sales price for each house Id in the test set
Experience (E): The Ames Housing dataset compiled by Dean De Cock. This is a dataset with 79 explanatory variables describing every aspect of residential
homes in Ames in Iowa.
Performance (P): Prediction accuracy, the closer the prediction to the actual sale price of the house sold. These are evaluated on the Root-Mean-Squared-Error
(RSME) between the logarithm of the observed sales price and the predicted value. The log is used to stop the skew between cheaper and more expensive
houses.
Assumptions
- The size of the house and location will matter to the model
- As Overall Quality of the house increases, the Sale Price also increases
- As ground living area increases, the sale price will increase
- As the building ages, it will decrease in value
Why solve this problem?
A house is typically the largest purchase that will be made in an individuals lifetime. It’s worth being well informed about what a house’s selling price would be,
be it for the individual or a broker/ mortgage provider.
How will I solve this problem?
Firstly, I need to figure out what type of house is being sold generally? Are there any trends that can be seen? The next step is to decide what columns to drop,
fill in null values, create a pipeline, vector assembler and start fitting the data to models. The models will then be assessed.
Data Exploration, Feature Engineering and Data Preparation
Data Exploration
Firstly I loaded in the dataset. I used spark.read.csv() to read in the data, with the settings that imported it as a Spark DataFrame, taking the first row as a
header, inferring the schema and specifying null values as “NA”. There is not a lot of information to be retrieved from this, so I started off with some basic
exploration. I checked the shape of the dataset which was (1460, 81) and printed the schema to check the inferred schema and took note of what was incorrect.
I then viewed some general information about the data, such as count, mean, min and max using df.describe(). As you can see below, immediately with the 
