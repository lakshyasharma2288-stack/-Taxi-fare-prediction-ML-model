# Taxi Fare Prediction using Machine Learning

## Project Overview

This project focuses on building a machine learning model to predict taxi fares based on trip-related features such as pickup and dropoff locations, passenger count, and time of travel. It demonstrates a complete end-to-end workflow, including data preprocessing, feature engineering, model training, and evaluation.

The objective is to create a predictive system similar to those used in real-world ride-hailing platforms.

---

## Problem Statement

Accurate taxi fare prediction is essential for improving pricing transparency and customer experience. Incorrect estimates can result in customer dissatisfaction and inefficient pricing strategies.

This project aims to solve this problem using regression-based machine learning techniques.

---

## Dataset Description

The dataset contains historical taxi trip records with the following features:

* pickup_datetime: Timestamp of the ride
* pickup_longitude & pickup_latitude: Pickup location coordinates
* dropoff_longitude & dropoff_latitude: Dropoff location coordinates
* passenger_count: Number of passengers
* fare_amount: Target variable (fare price)

---

## Machine Learning Pipeline

### Data Cleaning

* Removed missing and null values
* Filtered invalid geographic coordinates
* Handled outliers in fare and distance

---

### Feature Engineering

* Extracted time-based features such as hour, day, and month
* Calculated trip distance using the Haversine formula
* Removed irrelevant or noisy data

Feature engineering played a key role in improving model performance.

---

### Exploratory Data Analysis

* Analyzed distribution of fare values
* Studied relationship between distance and fare
* Observed patterns based on time features

---

### Model Building

#### Linear Regression

* Used as a baseline model
* Simple and fast
* Limited in capturing complex patterns

#### Random Forest Regressor

* Handles nonlinear relationships effectively
* More robust to noise and outliers
* Provides improved accuracy over linear models

---

### Model Evaluation

The following metrics were used:

* Mean Absolute Error (MAE)
* Root Mean Squared Error (RMSE)

Comparison summary:

* Linear Regression shows higher error due to underfitting
* Random Forest performs better due to its ability to capture complex feature interactions

---

## Key Insights

* Distance is the most important factor in fare prediction
* Time-based features influence pricing trends
* Linear models are not sufficient for real-world datasets
* Ensemble methods significantly improve accuracy

---

## Tech Stack

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib / Seaborn

