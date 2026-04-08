# Future-Stocks-Prediction

## Objective
This project aims to predict the **next day's closing price** of a stock using historical market data. It explores short-term price forecasting using regression-based machine learning models.

## Dataset
- **Source:** Yahoo Finance (via the `yfinance` library).
- **Ticker:** Apple Inc. (AAPL) - *Adjustable in the code*.
- **Features:** Open, High, Low, and Volume.
- **Target:** The Closing Price of the subsequent trading day.

## Methodology
1. **Data Fetching:** Downloading historical OHLCV data.
2. **Feature Engineering:** Shifting the 'Close' price to create a 'Target_Close' column for supervised learning.
3. **Data Splitting:** Using a non-shuffled split (80/20) to maintain the temporal order of time-series data.
4. **Modeling:**
   - **Linear Regression:** A baseline statistical model.
   - **Random Forest Regressor:** An ensemble learning method to capture non-linear relationships.
5. **Evaluation:** Assessing performance using the R-squared (R2) score.
6. **Visualization:** Comparing predicted vs. actual prices over the test period.

## Dependencies
- `yfinance`
- `pandas`
- `numpy`
- `matplotlib`
- `scikit-learn`
