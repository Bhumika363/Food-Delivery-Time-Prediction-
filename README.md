# 🍔 Food Delivery Time Prediction Using Linear Regression 📊

A machine learning-based prediction system designed to analyze food delivery data and estimate delivery time based on factors such as delivery distance, delivery person details, weather conditions, traffic level, order type, and vehicle type. The project implements both Simple and Multiple Linear Regression to understand the relationship between delivery conditions and delivery time.

## 📘 Project Overview

Food delivery time depends on several factors, including the distance between the restaurant and customer, traffic conditions, weather, vehicle type, and delivery person characteristics. **Food Delivery Time Prediction** analyzes these factors using a Kaggle food delivery dataset and applies Linear Regression techniques to predict delivery time.

The project follows a complete machine learning workflow, including data preprocessing, missing-value handling, geographical distance calculation, categorical encoding, feature selection, model training, evaluation, visualization, and prediction.

## 🧩 Features

- **Data Preprocessing:** Cleans the dataset and handles missing and invalid values before model training.
- **Haversine Distance Calculation:** Calculates geographical distance between restaurant and delivery location using latitude and longitude.
- **Feature Engineering:** Selects relevant numerical and categorical features for prediction.
- **One-Hot Encoding:** Converts categorical features such as traffic level, weather, order type, and vehicle type into numerical form.
- **Simple Linear Regression:** Predicts delivery time using delivery distance as the main feature.
- **Multiple Linear Regression:** Uses multiple delivery-related features to predict delivery time.
- **Model Evaluation:** Evaluates predictions using MAE, MSE, RMSE, and R² Score.
- **Data Visualization:** Uses graphs to analyze the relationship between distance and delivery time and compare actual and predicted values.
- **New Order Prediction:** Predicts delivery time for a new delivery distance.

## ⚙️ Components & Technologies

- **Python:** Core programming language used for data processing and machine learning.
- **Google Colab:** Development environment used to build and execute the project.
- **Pandas:** Used for data loading, cleaning, preprocessing, and analysis.
- **NumPy:** Used for numerical operations and array processing.
- **Matplotlib:** Used for generating data visualizations.
- **Scikit-learn:** Used for Linear Regression, data splitting, encoding, and model evaluation.
- **Linear Regression:** Machine learning algorithm used for delivery time prediction.

## 🧠 Working Principle

1. **Data Ingestion:** The Food Delivery Time dataset is loaded and analyzed using Pandas.
2. **Data Cleaning:** Missing values in categorical and numerical columns are handled using appropriate techniques such as mode and median imputation.
3. **Distance Processing:** Missing distance values are calculated using the Haversine Formula based on restaurant and delivery-location coordinates.
4. **Target Cleaning:** Invalid values such as `#VALUE!` in the target column are removed and valid delivery-time values are converted into numerical form.
5. **Feature Selection:** Relevant delivery, weather, traffic, order, vehicle, and distance-related features are selected.
6. **Feature Encoding:** Categorical features are converted into numerical values using One-Hot Encoding.
7. **Data Splitting:** The processed dataset is divided into training and testing sets using an 80:20 ratio.
8. **Model Training:** Simple Linear Regression is trained using distance, while Multiple Linear Regression uses multiple selected features.
9. **Model Evaluation:** The trained models are evaluated using MAE, MSE, RMSE, and R² Score.
10. **Prediction:** The Simple Linear Regression model is used to estimate delivery time for a new order based on its delivery distance.

## 📊 Results

The project achieved the following results on the available cleaned dataset:

### Simple Linear Regression

- **MAE:** 4.03 minutes
- **RMSE:** 4.62 minutes
- **R² Score:** 0.65

The trained regression equation was:

`Delivery Time = 8.84 + 1.41 × Distance (km)`

For a new delivery distance of **10 km**, the model predicted an approximate delivery time of **22.94 minutes**.

### Multiple Linear Regression

- **MAE:** 7.33 minutes
- **RMSE:** 9.56 minutes
- **R² Score:** -0.49

The results are based on the particular train-test split used in the project. After data cleaning, only **30 valid target records** were available, so the results are intended primarily for academic demonstration rather than real-world deployment.

## 📈 Visualization

The project includes visualizations to understand model behavior and delivery trends:

- **Distance vs Delivery Time:** Shows the relationship between delivery distance and delivery time along with the regression line.
- **Actual vs Predicted Delivery Time:** Compares actual delivery times with model predictions.

These visualizations provide a graphical understanding of the relationship between the input features and predicted delivery time.

## 🎯 Learning Outcomes

Through this project, the following Machine Learning concepts were implemented:

- Data preprocessing and cleaning
- Missing-value handling
- Outlier analysis
- Feature selection
- Feature encoding
- Haversine distance calculation
- Train-test splitting
- Simple Linear Regression
- Multiple Linear Regression
- Model prediction
- Regression evaluation metrics
- Data visualization

## 🚀 Future Enhancements

- **Larger Dataset:** Use a larger and cleaner dataset to improve model reliability.
- **Real-Time Traffic Integration:** Include live traffic information for more accurate predictions.
- **Weather API Integration:** Incorporate real-time weather conditions.
- **Advanced Machine Learning:** Compare Linear Regression with Decision Tree, Random Forest, and other regression algorithms.
- **Real-Time GPS:** Use GPS data for dynamic distance calculation.
- **Restaurant Preparation Time:** Include food preparation time as an additional prediction factor.
- **Web Application:** Develop an interactive web interface for real-time delivery time prediction.
- **Model Deployment:** Deploy the trained model for practical food delivery applications.

## 🏁 Conclusion

The **Food Delivery Time Prediction Using Linear Regression** project demonstrates how Machine Learning can be applied to estimate food delivery time using real-world delivery-related factors.

The project successfully implements the complete workflow from **data preprocessing and feature engineering to model training, evaluation, visualization, and prediction**. Simple Linear Regression establishes a clear relationship between delivery distance and delivery time, while Multiple Linear Regression demonstrates how multiple factors can be incorporated into a prediction model.

The project provides a practical understanding of **Linear Regression, data preprocessing, feature encoding, model evaluation, and prediction**, while also providing a foundation for developing more advanced and real-time food delivery prediction systems.

## 📄 License

© 2026 **Bhumika**. All Rights Reserved.

This project and its contents are the intellectual property of the author. No part of this repository may be copied, modified, distributed, reproduced, or used for commercial or academic purposes without prior written permission from the author.

### 🌐 Keywords

Machine Learning | Linear Regression | Multiple Linear Regression | Python | Data Science | Food Delivery | Delivery Time Prediction | Pandas | NumPy | Scikit-learn | Matplotlib | Google Colab | Data Preprocessing | One-Hot Encoding | Haversine Formula
