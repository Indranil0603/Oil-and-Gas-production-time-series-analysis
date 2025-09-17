Here is a README template for your project, including instructions to add the model comparison image:

***

# Oil Production Forecasting Model Comparison

## Overview
This project evaluates and compares the forecasting performance of three models applied to oil production data:
- Facebook Prophet (additive time series model)
- ARIMA (seasonal statistical model)
- LSTM (deep learning recurrent network)

The purpose is to identify the best model for predicting oil production, balancing accuracy, interpretability, and computational cost.

## Dataset
- Historical oil production data for PADD 2 (Midwest) regions.
- Features engineered include lagged values, rolling window statistics, and temporal components.

## Modeling Approach
- Prophet, ARIMA, and LSTM models are trained and hyperparameter-tuned using Bayesian optimization (Optuna).
- Evaluation metrics include MAE, MSE, RMSE, MAPE, and R².
- Results are saved in a standardized format to enable fair comparison.

## Results Summary
- LSTM shows the best forecasting accuracy with lowest errors and a positive R².
- ARIMA provides a robust statistical benchmark with moderate performance.
- Prophet is highly interpretable and fast to deploy but less accurate in complex scenarios.

## Model Comparison Metrics

| Model   | MAE     | MSE       | RMSE    | MAPE (%) | R²      |
|---------|----------|----------|---------|----------|---------|
| Prophet | 665.504  | 543887.987 | 737.488 | 37.939   | -11.590 |
| ARIMA   | 194.801  | 72705.759  | 269.640 | 9.916    | -0.683  |
| LSTM    | 79.129   | 15692.829  | 125.271 | 11.156   | 0.632   |

## Final Recommendation
- Use LSTM for production when accuracy is critical.
- Use Prophet for quick deployment and stakeholder communication.
- Use ARIMA as a reliable statistical baseline.

## Visualizing Model Comparison
The image below presents the forecast vs. actual production values for each model, highlighting their relative performance over time:

