# Analysis and Prediction on Auto.csv

# Overview

This notebook implements an exploratory data analysis and predictive modeling assignment focused on the "Auto" dataset. The analysis includes data preprocessing,feature engineering and building models to predict car attributes based on fuel efficiency.

# Project Description

The assignment focuses on:

1. Exploring the relationship between features such as weight, horsepower, displacement and fuel efficiency (miles per gallon, mpg).

2. Creating a binary classifcation variable (mpg01) based on whether a car's mpg is above or below the median value.

3. Splitting the dataset into training and test sets for predictive analysis.

4. Building and evaluating machine learning models, including k-Nearest Neighbors (kNN) to classify cars based on fuel efficiency.

# Setup and Dependencies

 **Libraries**

 The following Python libraries are required to run the notebook:

 1. pandas

 2. numpy

 3. matplotlib

 4. seaborn

 5. scikit-learn

**Dataset**

The dataset used in this assignment is the "Auto.csv" file. Ensure the dataset is available in the working directory before running the notebook.

# Data Preprocessing

1. Load the dataset using pandas.

2. Inspect and clean the dataset, handling missing or anomalous values.

3. Create a binary classification variable mpg01:
   
     1. Assign "1" if mpg is above the median.
  
     2. Assign "0" otherwise.
  
 5. Split the data into training (70%) and test sets (30%).

# Exploratory Data Analysis (EDA)

Key findings from the visualizations and statistical summaries:

1. **Weight and Displacement** : Negatively correlated with mpg01. Lighter cars tend to have higher gas mileage.

2. **Horsepower** : Higher horsepower correlates with lower gas mileage.

3. **Cylinders** : Fewer cylinders are associated with higher gas mileage.

4. **Year** : Newer cars are generally more fuel-efficient.

5. **Acceleration** : Less significant difference observed between mileage categories.

# Predictive Modeling

1. k-Nearest Neighbors (kNN):

    1. Tested various values of K.
  
    2. Found the optimal K with minimal test error.
  
2. Error Analysis:

    1. Smaller K values may lead to overfitting.
  
    2. Recommended values of K = 3 or 7.
  
# Results and Observations 

1. The best test error was observed when K = 1. However, this may overfit the training data.

2. Features such as weight, displacement, horsepower, cylinders, and year were most predictive of mpg01.
