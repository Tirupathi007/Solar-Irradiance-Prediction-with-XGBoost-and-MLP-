# **Solar Irradiance Prediction**

This project predicts solar irradiance using meteorological data from HI-SEAS (Sep-Dec 2016) with XGBoost and MultiLayer Perceptron (MLP) models.

## **Project Overview**
- **Objective**: Forecast solar radiation (W/m²) using features like temperature, humidity, and wind.
- **Dataset**: HI-SEAS weather data with 32,661 records from Kaggle.

## **Methodology**
- **Preprocessing**: Loaded data, handled missing values, and extracted features from timestamps.
- **Feature Selection**: Used Correlation Matrix, SelectKBest, and ExtraTreesClassifier to identify key predictors.
- **Feature Engineering**: Applied BoxCox, Log, Min-Max, and Standard transformations.
- **Models**:
  - XGBoost: Ensemble model for regression.
  - MLP: Neural network with Dense, Dropout, and Adam optimizer.
- **Data Split**: Train-test split with standardization.

## **Results**
- **MLP Performance**: Achieved Mean Absolute Error (MAE) of 40.68 W/m².
- **Feature Importance**: Temperature and time-based features were most predictive.

## **Recommendations**
- Prioritize MLP for accurate predictions; refine XGBoost with hyperparameter tuning.
- Explore additional temporal features to enhance model performance.
