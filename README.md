# Stock Price Prediction using Linear Regression

This project focuses on predicting the **next day's stock closing prices** using historical data from the **Nifty50 dataset**. The model is built using **Linear Regression** and is designed to process **multiple stock CSV files** in a batch.

## Objective

- Predict the next-day stock price based on current day’s closing price.
- Evaluate model performance using **Mean Squared Error (MSE)** and **R² Score**.
- Visualize actual vs predicted stock prices.

## Machine Learning Algorithm

- **Linear Regression** – A simple and interpretable regression model used for forecasting the next day’s closing price.

## Dataset

- Source: [Kaggle - Nifty50 Stock Market Data](https://www.kaggle.com/datasets/rohanrao/nifty50-stock-market-data)
- Format: Multiple CSV files (one per stock)
- Features Used: `Close`
- Label: `Next_Close` (shifted one day forward)

## Tools & Libraries

- **Python**
- **Google Colab**
- `pandas`, `os`, `matplotlib`
- `sklearn.linear_model`, `sklearn.metrics`, `train_test_split`

## How It Works

1. Reads all CSV files from the specified folder
2. Checks for valid structure (`Close` column)
3. Creates a new column `Next_Close` for the next day’s price
4. Splits data into training and testing sets (80-20)
5. Trains a Linear Regression model
6. Evaluates performance using MSE and R²
7. Visualizes actual vs predicted prices for each stock

## Sample Output

-  **Mean Squared Error (MSE):** ~11–15  
-  **R² Score:** ~0.90–0.95  
-  Visual graphs show actual vs predicted trends for each stock

## Folder Structure
- README File
- python file
- Project Report
- Project Presentation
- Dataset folder

## Notes

- Files with missing or insufficient data are automatically skipped.
- No shuffling is done to preserve the time-series nature of data.

## Future Enhancements

- Use additional features like `Open`, `High`, `Low`, `Volume`
- Add support for other models (Random Forest, LSTM)
- Forecast multiple days ahead

## Group Members
- Akash
- Aniruddha Singh
- Akash
- Anshul Anand
- Aditi Singh


