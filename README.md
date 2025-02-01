# Stock-Prediction

#Overview:

This project utilizes a Long Short-Term Memory (LSTM) neural network to predict stock prices based on historical stock data. The dataset is fetched using Yahoo Finance, preprocessed, and then used to train the LSTM model.

#Dependencies:
Make sure you have the following Python libraries installed before running the script:
pip install numpy pandas matplotlib yfinance scikit-learn tensorflow keras

#Dataset:
The stock price data is fetched using the yfinance library. The script downloads historical stock data for the specified company within a given date range.

#Data Preprocessing:
Extracts the closing prices.
Calculates 100-day and 200-day moving averages.
Normalizes the data using MinMaxScaler.
Splits the dataset into training (80%) and testing (20%) sets.

#Model Architecture:
Four LSTM layers with increasing units (50, 60, 80, 120) and ReLU activation.
Dropout layers to prevent overfitting.
A Dense layer as the output for the predicted stock price.

#Training:
The model is compiled with the Adam optimizer and Mean Squared Error (MSE) loss function.
Trained for 50 epochs with a batch size of 32.

#Evaluation & Prediction:
The model is tested on unseen data.
Predictions are plotted against actual prices for visualization.
