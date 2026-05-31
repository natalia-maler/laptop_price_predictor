# Laptop Price Prediction using Machine Learning
## Project Overview

This project focuses on predicting laptop prices using machine learning techniques.
The dataset contains technical specifications of laptops such as RAM, CPU, GPU, storage type, display resolution, operating system, and screen characteristics.

The main goal of the project is to build and compare multiple regression models capable of estimating laptop prices based on hardware configuration and technical features.

## Dataset
The dataset includes information about laptops such as:
- Company
- Laptop type
- RAM
- CPU
- GPU
- Storage configuration
- Screen resolution
- Operating system
- Weight
- Price

## Data Preprocessing
Several preprocessing and feature engineering steps were applied before training the models.

Cleaning and Transformation
- Removed unnecessary columns
- Converted RAM and storage values into numerical format
- Extracted screen resolution values X_res, Y_res
- Converted categorical features into numerical representations

## Feature Engineering
Additional features were created to improve model performance.

- Touchscreen detection: a binary feature indicating whether the laptop has a touchscreen display.
- IPS display: a binary feature indicating IPS panel usage.
- PPI (Pixels Per Inch): calculated using screen resolution and screen size to better represent display quality.
- Storage separation: the storage column was decomposed into: HDD, SSD, Hybrid Storage, Flash Storage
- GPU Brand extraction: rxtracted GPU manufacturer from the GPU column.
- Operating system categorization
Grouped operating systems into: Windows, Mac, Others / Linux / No OS

## Exploratory Data Analysis (EDA)
Several visualizations were used to better understand the dataset and relationships between features and laptop prices.

Examples include:
- price distribution plots
- company vs price comparisons
- correlation analysis
- feature importance analysis

## Machine Learning Models
Multiple regression algorithms were trained and compared:
- Linear Regression
- Ridge Regression
- Lasso Regression
- K-Nearest Neighbors
- Decision Tree Regressor
- Support Vector Regressor (SVR)
- Random Forest Regressor
- Extra Trees Regressor
- AdaBoost Regressor
- Gradient Boosting Regressor
- XGBoost Regressor

## Model evaluation
Models were evaluated using: 
- R^2 Score: measures how well the model explains price variance.
- MAE: measures average prediction error.

## Prediction System
The trained models can predict prices for completely new laptop configurations.
Example input: RAM, CPU, GPU, SSD, screen characteristics, operating system

The model then estimates the expected laptop price.

## Prediction Range
Instead of returning a single fixed value, the project also introduces a prediction range.

Example:

Estimated Price: 85.000 - 95.000

This provides a more realistic business-oriented interpretation of model uncertainty and estimated market value.

## Conclusion
This project demonstrates a complete end-to-end machine learning workflow for price prediction problems.

The final solution is capable of estimating laptop prices based on technical specifications and can serve as a foundation for real-world pricing systems or recommendation engines.
