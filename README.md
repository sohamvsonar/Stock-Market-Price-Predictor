
# Stock Market Price Predictor

## 1. Overview

This repository contains a Python implementation of a stock market price predictor using LSTM (Long Short-Term Memory) neural networks. The predictor is designed to forecast stock prices based on historical data. The LSTM model is built using TensorFlow and Keras, and the stock price data is fetched using the Yahoo Finance API. If you have any questions please feel free to reach me out via mail at soham.sonar427@gmail.com or on linked at https://www.linkedin.com/in/sohamsonar23/, Thank You!


## 2. Requirements:

- Python 3.6 or higher
- Required Python packages can be installed using the following command:

  ```bash
  pip install numpy matplotlib pandas pandas_datareader scikit-learn tensorflow yfinance

## 3. Usage

### 1. Clone the repository:
    ```bash
    git clone https://github.com/sohamvsonar/Stock-Market-Price-Predictor.git
### 2. Install the required packages

### 3. Run the predictor script:
    ```bash
    python Stock-Market-Price-Predictor.py

The script downloads historical stock price data, preprocesses it using Min-Max scaling, trains an LSTM model, and visualizes the predicted vs. actual prices.

## Configuration
1. The company variable in the script is set to 'AAPL' by default. You can change it to the desired stock symbol.
2. Adjust the start and end variables to set the training data timeframe.
3. Fine-tune the LSTM model architecture and training parameters as needed.

## Technical Details
1. Data Preprocessing:
-   The historical stock prices are fetched using the Yahoo Finance API (yfinance).
-   Min-Max scaling is applied to normalize the closing prices between 0 and 1.

2. LSTM Architecture:
-   The model consists of three LSTM layers with 50 units each, followed by dropout layers to prevent overfitting.
-   The final layer is a Dense layer with a single unit, predicting the next day's stock price.

3. Training:
-   The model is compiled with the Adam optimizer and mean squared error loss function.
-   Training is performed for 25 epochs with a batch size of 32.

4. Testing:
-   Test data is fetched from the specified start date to the current date.
-   Actual and predicted stock prices are visualized using Matplotlib.

## ScreenShot:
![](https://github.com/sohamsonar427/Stock-Market-Price-Predictor/blob/main/Screenshots/SS.jpg)

![](https://github.com/sohamsonar427/Stock-Market-Price-Predictor/blob/main/Screenshots/SS1.jpg)

## Example Output:
-   The script generates a plot displaying actual and predicted stock prices.

## Acknowledgements:
-   The code is inspired by various LSTM-based stock price prediction implementations.

## Research Paper:
1. ESTIMATING STOCK PRICES USING LSTM:
-   Published a research paper in Dickensian Journal Volume 22, ISSUE 6, 2022 ISSN: 0012-2440.
2. FORECASTING EQUITY PRICES USING LSTM ALGORITH:
-   Published in IJCRT Journal VOLUME 9, ISSUE 12 December 2021 ISSN: 
2320-2882.

## Disclaimer:
-   This project is for educational and informational purposes only. It should not be considered financial advice.
