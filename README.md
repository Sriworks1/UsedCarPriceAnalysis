# Used Car Price Analysis - Application #2

## Overview & Goal

In this application, we will explore a dataset from kaggle. The original dataset contained information on 3 million used cars. The provided dataset contains information on 426K cars to ensure speed of processing. Our goal is to understand what factors make a car more or less expensive. As a result of this analysis, we should provide a clear recommendations to our client -- a used car dealership -- as to what consumers value in a used car.

## Business Understanding

Our customer is a used car dealer. It is important for him to know what feature of a car customer values the most and how it impacts the car price. 

With a Car's dataset given, the business goal is to understand the attributes that impact sales price of used cars and be able to predict the car prices. From the data standpoint, The objective is to:

1. Identity the top features that influence the car price
2. Build a predictive model with those features. We will use various data cleansing and machine learning techniques to identify the same.

## Data Understanding

| Field | Description |
| ----- | ----------- |
| ID | An identifier or unique identifier for each entry in the dataset.|
| Region | The region or location where the vehicle is listed for sale.|
| Price| The price of the vehicle listed for sale|
| Year | The manufacturing year of the vehicle.|
| Manufacturer| The manufacturer or brand of the vehicle.|
| Model| The model name or number of the vehicle.|
| Condition| The condition or state of the vehicle (e.g., excellent, good, fair).|
|Cylinders| The number of cylinders in the vehicle's engine|
|Fuel| The type of fuel the vehicle uses (e.g., gasoline, diesel, electric).|
|Odometer| The number of miles or kilometers the vehicle has been driven.|
|Title Status| The status of the vehicle's title (e.g., clean, salvage, rebuilt).|
|Transmission| The type of transmission in the vehicle (e.g., automatic, manual).|
|VIN| The Vehicle Identification Number, a unique identifier for the vehicle.|
|Drive| The type of drive or drivetrain in the vehicle (e.g., 2-wheel drive, 4-wheel drive).|
|Size| The size or class of the vehicle (e.g., compact, mid-size, full-size).|
|Type| The body type or style of the vehicle (e.g., sedan, SUV, truck).|
|Paint Color| The color of the vehicle's exterior paint.|
|State| The state where the vehicle is listed for sale.|

![Data Info](/images/df_info.png)

### Check for Missing values

There are a lot of missing values we could drop in prep phase.

![Missing Values](/images/missing_values.png)


### Check for outliers

Price column has outliers that could be removed in data prep. The below plots show the same.

![Price Outlier](/images/price_outliers.png)

### Explore price by category columns

![Price By Categories](/images/price_by_category.png)


## Data Preparation

Do basic data cleanup like 

1. Remove duplicates
2. Remove null values
3. Set Id as index.
4. Remove VIN Column in leu of Id column

![Basic Cleanup](/images/base-cleanup.png)

Now, Fill missing values with estimators

![Imputer](/images/imputer.png)


