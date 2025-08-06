# ''Arev-Arev ek-ek'' - Weather Forecast Prediction Model  

## Overview

   This project builds and evaluates a **linear regression model** to predict the **temperature of the next hour throughout 2022** using historical weather data. The goal is to capture short-term temperature dynamics with a simple and interpretable model. Just like giving your computer a weather crystal ball — but make it powered by math.

You’ll find clean data processing, smart feature handling, and solid performance evaluation, all wrapped into a single streamlined notebook.

---

## Workflow Summary

After data preprocessing and feature engineering, these steps follow:

1. **Data Splitting**  
   The data is split into three sets:
   - `training`: used to train the model
   - `validating`: used to tune and test during training
   - `testing`: used to evaluate final model performance

2. **Feature & Target Separation**  
   - Features: all columns *except* `next_hour_pred`
   - Target: the `next_hour_pred` column (temperature for the next hour)

3. **Normalization**  
   - Only **features** are scaled using `StandardScaler`.
   - Target column remains untouched.

4. **Model Training**  
   - A simple yet effective `LinearRegression` model from scikit-learn is trained on the scaled training features.

5. **Evaluation**  
   - Model predictions are compared to actual values using:
     - **RMSE** (Root Mean Squared Error)
     - **MAE** (Mean Absolute Error)
     - **R² Score** (Coefficient of Determination)

6. **Prediction Results**  
   - Actual vs. Predicted values are saved in a `.csv` file for further analysis.

---

## Files

- `WeatherModel_SereenSipan.ipynb`: Main notebook with all preprocessing, model training, and evaluation steps.
- `Predictions_for_2022.csv`: Contains 3 columns - actual, predicted, and absolute difference values for the test set.
- `NYC_Weather_2016_2022.csv`: The input data file the model was trained on.
---

## TA-DAA! :D
