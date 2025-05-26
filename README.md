# Bitcoin-price-prediction
Bitcoin Price Prediction
Accurately anticipating asset prices is an important but difficult task in the highly unpredictable cryptocurrency market. The goal of this project is to use machine learning models to create a comprehensive end-to-end system for trading signal generation, technical indicator analysis, Bitcoin price prediction, and risk assessment. The system offers perceptive, data-driven forecasts and visualizations that support strategic decision-making by combining statistical indicators, historical market data, and ensemble learning techniques.
Objectives:
1.Data Collection:
Automatically retrieve up-to-date historical data for Bitcoin (BTC-USD) using the yfinance API.

2. Feature Engineering:
Generate powerful predictive features from raw data using technical indicators like:
•	RSI (Relative Strength Index)
•	MACD (Moving Average Convergence Divergence)
•	SMA (Simple Moving Averages)
•	Bollinger Bands
•	Lag-based returns and volatility metrics

4.   Model Building & Evaluation:
Train and evaluate different machine learning regression models:
•	Linear Regression (Baseline model)
•	Random Forest Regressor (Bagging Ensemble)
•	XGBoost Regressor (Boosting Ensemble)
Each model is tested using metrics like:
•	RMSE (Root Mean Squared Error)
•	MAE (Mean Absolute Error)
•	R² Score (Coefficient of Determination)

6. Visualization:
Interactive charts using Plotly to display:
•	BTC price history
•	Moving averages and RSI plots
•	Model performance comparison
•	Predicted vs actual price graphs

8.  Prediction System:
Predict the next BTC price using the best-performing model, and calculate the percentage change from the current price.






Pipeline
1. Data Pipeline
•	Download historical BTC data from Yahoo Finance for 2 years.
•	Reset the index, parse dates, and preview closing prices.
2. Feature Engineering
•	Calculate percent returns, lagged prices, price momentum.
•	Technical indicators like:
o	SMA: Used for identifying bullish/bearish trends.
o	RSI: Momentum oscillator for identifying overbought/oversold zones.
o	MACD: Measures momentum and trend direction.
o	Bollinger Bands: Volatility-based band system.
o	High/Low ratio, Volume trend, Volatility metrics (7-day, 30-day).
3. Model Training
•	Features are split into training and test sets (80-20 split).
•	Scaling is applied where required (e.g., Linear Regression).
•	Three models are trained:
o	Linear Regression: Fast and interpretable baseline.
o	Random Forest: Reduces overfitting by averaging decision trees.
o	XGBoost: A boosting method that excels in tabular regression tasks.
•	Evaluation metrics calculated for each model.
4. Visualization
•	Interactive price and prediction graphs.
•	Comparison bar charts for RMSE and R².


5. Prediction
•	Uses the best-performing model (lowest RMSE).
•	Predicts the next price and calculates the percentage change from the current price.

Summary:

This project delivers a robust, end-to-end Bitcoin price prediction and trading decision support system by combining financial data analysis, technical indicators, and machine learning models. It seamlessly integrates data collection, feature engineering, model training, visualization, and risk assessment into a single workflow. By leveraging algorithms like Linear Regression, Random Forest, and XGBoost, along with key indicators such as RSI, MACD, and Bollinger Bands, the system provides accurate price forecasts and actionable trading signals. With added capabilities for real-time predictions, performance comparison, and risk evaluation, this project serves as a practical and insightful tool for traders, investors, and data scientists aiming to navigate the dynamic world of cryptocurrency markets.


![Screenshot 2025-05-26 230647](https://github.com/user-attachments/assets/f5f87e09-2948-484c-aa9b-7e239319ad13)


![image](https://github.com/user-attachments/assets/71e6187c-aa8e-4ce5-9362-f2ecc8b39967)
