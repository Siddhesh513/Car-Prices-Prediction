#  Car Prices Prediction 

## Introduction

There are a lot of __car manufacturers__ in the US. With the development of manufacturing units and tests, there are a lot of cars being manufactured with a lot of features. Therefore, innovators are coming with the latest developments in the field and they are ensuring that the drivers get the best experience going on a ride in these cars. 


## Business Contraints/Key Performance Metrics

However, one of the challenging aspects of running the sales for cars is to accurately give the __best price__ for cars which ensures that a lot of people buy them and there is a great demand because of this price. Their are many Factors that influence the price of cars such as __mileage__, __car size__, __manufacturer__ and many others as well. But for humans to comprehensively decide the price is difficult especially when there are a lot of these features that influence the price. One of the solutions to this challenge is to use __machine learning__ and __data science__ to understand the insights and make valuable predictions which generate profits for the companies.  

<h2> Data Source</h2>

The data set that we will be working on is quite a big dataset which contain about __10,000__ data points where again we would be dividing that into training set and the test set. Having a look at some of the cars that we are always excited to use in our daily lives, it is better to understand how these cars are being sold and their average prices. You can check the dataset that I will be using for the process of predicting the prices of cars.
Below is the link.

https://www.kaggle.com/CooperUnion/cardataset

## Machine Learning and Deep Learning

<p>In the last decade, <strong>machine learning</strong> and <strong>deep learning</strong> have exploded in popularity. It would be really beneficial if we could estimate automobile pricing based on a few characteristics such as horsepower, make, and other characteristics. Consider how a corporation might set a car's pricing based on factors such as make, <strong>horsepower</strong>, and <strong>mileage</strong>. It could do so with the assistance of <strong>machine learning algorithms</strong> that would assist it in determining the car's price. This would ensure that the corporation sets the correct quantity in order to maximize profits while doing so. As a result, the machine learning models that we will be using will ensure that the correct pricing is established for new cars, saving car manufacturers a significant amount of money.
We'd be working with car price prediction data and looking for different types of car predictions. We'd start by visualizing the data and understanding some of the key elements for making predictions. To get the average price of the car in question, we'll use a variety of regression algorithms.
 </p>

We would be working with the car prices prediction data and looking for the predictions of different kinds of cars. We would be first visualizing the data and understanding some of the information that is very important for predictions. We would be using different regression techniques to get the average price of the car under consideration.

## Metrics

We will be Predicting the car prices is a __continuous machine learning problem__. Therefore, the following metrics that are useful for regression problems are taken into account. Below are the __metrics__ that were used in the process of predicting of car prices.

* [__Mean Squared Error (MSE)__](https://scikit-learn.org/stable/modules/generated/sklearn.metrics.mean_squared_error.html)
* [__Mean Absolute Error (MAE)__](https://scikit-learn.org/stable/modules/generated/sklearn.metrics.mean_absolute_error.html)

## Exploratory Data Analysis (EDA)

In this section of the project, the data is explored to see the patterns and trends and observe interesting insights. Below are some interesting observations generated.

* A large number of cars were from the manufacturer __'Chevrolet'__ followed by __'Ford'__. 
* The total number of cars manufactured during the year __2015__ were the highest in all the years found on the data.
* There were many missing values for __'Market Category'__ feature and a few missing values for the features __'Engine HP'__ and __'Engine Cylinders'__.
* The average prices of the cars were the highest in the year __2014__ and lowest in the year __1990__ from the data. 
* The prices of __'Bugatti'__ manufacturer are extremely high compared to the other car manufacturers.  
* __'Bugatti'__ manufacturer also had an extremely high value for the horsepower (HP) based on the graphs in the notebook.
* There is a __negative correlation__ between the feature __'City Mileage'__ and other features such as __'Engine Cylinders'__ and __'Engine HP'__. This is true because higher the mileage of the car, there is a higher probability that the total number of cylinders and engine horsepower would be low. 

## Machine Learning Models 

We have to be using various machine learning models to see which model reduces the __mean absolute error (MAE)__ or __mean squared error (MSE)__ on the cross-validation data respectively. Below are the various machine learning models used. 

| __Machine Learning Models__| __Mean Absolute Error__| __Mean Squared Error__|
| :-:| :-:| :-:|
| [1. Linear Regression](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LinearRegression.html)| 6737| 364527989|
| [2. Support Vector Regressor](https://scikit-learn.org/stable/modules/generated/sklearn.svm.SVR.html)|	22525|	2653742304|
|	[3. K Nearest Regressor](https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.KNeighborsRegressor.html)|	4668|	198923161|
|	[4. PLS Regression](https://scikit-learn.org/stable/modules/generated/sklearn.cross_decomposition.PLSRegression.html)|	6732|	364661296|
|	[5. Decision Tree Regressor](https://scikit-learn.org/stable/modules/generated/sklearn.tree.DecisionTreeRegressor.html)|	__3327__|	135789622|
|	[6. Gradient Boosting Regressor](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.GradientBoostingRegressor.html)|	4432|	175275369|
|	[7. MLP Regressor](https://scikit-learn.org/stable/modules/generated/sklearn.neural_network.MLPRegressor.html)|	6467|	250908327|

## Outcomes

* The best model that was performing the best in terms of __mean absolute error (MAE)__ and __mean squared error (MSE)__ was __Decision Tree Regressor__.
* __Exploratory Data Analysis (EDA)__ revealed that __Bugatti manufacturer's prices__ were significantly higher than the other manufacturers. 
* __Scatterplots__ between the __actual prices__ and __predicted prices__ were almost __linear__, especially for the __Decision Tree Regressor__ model.

## Future Scope

* It would be great if the best __machine learning model (Decision Tree Regressor)__ is integrated in the live application where a __seller__ is able to add details such as the __manufacturer__, __year of manufacture__ and __engine cylinders__ to determine the best price for cars that generates __large profit margins__ for the seller. 
* Adding __additional data points__ and __features__ could help in also better determining the best prices for the latest cars as well. 
