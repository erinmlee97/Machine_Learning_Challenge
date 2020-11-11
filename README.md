# Machine_Learning_Challenge

## Background

Over a period of nine years in deep space, the NASA Kepler space telescope has been out on a planet-hunting mission to discover hidden planets outside of our solar system.

To help process this data, you will create machine learning models capable of classifying candidate exoplanets from the raw dataset.

## Instructions

### Preprocess the Data

* Preprocess the dataset prior to fitting the model.
* Perform feature selection and remove unnecessary features.
* Use `MinMaxScaler` to scale the numerical data.
* Separate the data into training and testing data.

### Tune Model Parameters

* Use `GridSearch` to tune model parameters.
* Tune and compare at least two different classifiers.

## Model 1: SVM

* For the model, I first stared by reading the data into a DataFrame and cleaning the data for values I did not need and scaled the data.
* I then defined what features I would use for x when creating my model. I set these values equal to X and used koi_disposition for my y.
* Data Scores
    * Training Data Score: 0.8916650772458516
    * Testing Data Score: 0.8947368421052632
* I then used  `GridsearchCV` to tune my model by changing `C` and `gamma`. This gave me a best score of 0.8888044957393081.

## Model 2: Linear Regression

* For the model, I also stared by reading the data into a DataFrame and cleaning the data for values I did not need and scaled the data.
* Data Scores
    * Training Data Score: 0.887659736791913
    * Testing Data Score: 0.8895881006864989
* I then used  `GridsearchCV` to tune my model by changing `C` and `gamma`. This gave me a best score of 0.8844179116424948.

## Analysis for Model 1 & 2
* Neither one of my models were significantly affected by changing `C` and `gamma`.
* There were no significant differences between my SVM model and my Linear Regression model. However, it looks like the SVM model performs slightly better than the Linear Regression model. 

