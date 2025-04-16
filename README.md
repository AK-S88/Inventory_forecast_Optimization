# 📦 Inventory Forecast Optimization – Python (Simulated Data)

This project demonstrates how predictive analytics and supply chain simulations can optimize inventory management and improve forecasting accuracy. The analysis uses simulated data modeled after real-world manufacturing environments, with a focus on semiconductor-style supply chain complexity.

## 📊 Project Overview

- **Objective:** Forecast demand and optimize inventory using statistical models and machine learning (ARIMA & LSTM).
- **Tools Used:** Python, Pandas, ARIMA (statsmodels), LSTM (TensorFlow), Tableau (dashboard), Matplotlib, SAP BI logic.
- **Focus Product:** A1 from a simulated fab-based inventory dataset.

# 🗃️ Dataset

- `inventory_data.csv`: Contains current inventory, safety stock, reorder points, and lead times for various products.
- `demand_signals.csv`: Contains weekly demand forecasts for each product over a 52-week period.

## 📈 KPIs (Product A1)

| KPI                   | Value       | Definition                                                                 |
|------------------------|-------------|------------------------------------------------------------------------------|
| **Stockout Rate**      | 96.15%      | % of weeks when demand couldn’t be met due to low inventory                 |
| **Average Inventory**  | 3.94 units  | Average number of units available across all weeks                          |
| **Reorder Frequency**  | 51 times    | Number of reorder events triggered based on reorder points                 |
| **Service Level**      | 3.85%       | % of weeks where full demand was met                                       |

> ⚠️ High stockout rate and low service level indicate poor planning despite frequent reorders. Forecasting is essential.

## 📉 ARIMA Demand Forecast

- ARIMA(1,1,1) model was trained on 80% of the data.
- Forecasted demand closely followed the actual trend with a Root Mean Squared Error (**RMSE**) of ~22 units.

## 🤖 LSTM Forecast (Neural Network)

- An LSTM model (4-week lookback) was trained to capture temporal patterns.
- Prediction curve aligns closely with the real demand but requires more data and tuning for production use.


## 📊 Visualizations

- **Inventory vs Forecasted Demand:** Time-based view of inventory depletion vs demand signal.
- **KPI Bar Chart:** Summarizes the simulation outcomes (stockouts, reorders, service rate).


*Created by Abhishek Kumar Singh – Business Analytics & Machine Learning @ UMass Lowell*

