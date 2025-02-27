# Rusty Bargain Predictive Model

## Overview
Rusty Bargain's used car sales service is developing an application to enhance customer engagement by providing quick car valuations. The model leverages historical data including technical specifications, trim versions, and prices to estimate the market value of used cars accurately. This project emphasizes prediction quality, prediction speed, and training time as key performance metrics.

## Technologies Used
- **Python**: Primary programming language
- **Pandas & NumPy**: Data manipulation and numerical computation
- **Matplotlib & Seaborn**: Data visualization
- **Scikit-Learn**: Machine learning algorithms and model evaluation
- **LightGBM**: Gradient boosting framework used for efficient modeling
- **Jupyter Notebook**: Interactive development environment

## Key Findings
- **Prediction Quality**: LightGBM offered the most accurate predictions with the lowest RMSE (Root Mean Squared Error).
- **Speed of Prediction**: Decision Tree was the fastest in making predictions, though it sacrificed some accuracy compared to LightGBM.
- **Training Time**: Decision Tree models were the quickest to train, while Random Forest models took the longest.

## Model Performance
- The **LightGBM** model performed best in terms of RMSE, achieving an RMSE of 1619.2757, which indicates a high level of accuracy in predicting car prices.
- **Random Forest** and **Decision Tree** models were also evaluated, with Random Forest providing a close performance to LightGBM in terms of RMSE.
- The speed of making predictions was fastest with the Decision Tree model, suitable for real-time applications.

## Conclusions
The analysis indicates that LightGBM is the most effective model for predicting used car prices accurately within Rusty Bargain's application. It offers an excellent balance between accuracy and computational efficiency. For real-time prediction requirements, Decision Trees offer a viable alternative with faster prediction times.

