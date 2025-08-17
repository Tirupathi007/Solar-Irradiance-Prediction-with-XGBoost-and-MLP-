# **Solar Irradiance Prediction**

This project predicts solar irradiance using meteorological data from the HI-SEAS weather station (Sep-Dec 2016).

## **Project Overview**
- **Objective**: Forecast solar radiation (W/m²) using XGBoost and MLP models.
- **Dataset**: HI-SEAS data with features like temperature, humidity, pressure, wind speed, and direction.

## **Methodology**
- **ETL & EDA**: Loaded data, performed data wrangling, and used SelectKBest to identify key features.
- **Data Transformations**: Applied Box-Cox, Log, Min-Max scaling, and standardization for preprocessing.
- **Feature Selection**: Used Correlation Matrix, SelectKBest, and ExtraTreesClassifier to select relevant features.
- **Models**:
  - XGBoost: Tree-based model for regression.
  - MLP: Neural network with Dense, Dropout, and Activation layers.

## **Results**
- **XGBoost**: Achieved R² of 0.93, outperforming other models.
- **MLP**: Recorded MAE of 40.68 on test set.
- **Key Features**: Temperature and humidity identified as top predictors via SelectKBest.

## **Recommendations**
- Deploy XGBoost for high-accuracy solar irradiance predictions.
- Optimize MLP architecture for improved performance.
