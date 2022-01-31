# AriStocks
In this repository, different RNN models (LSTM, BiLSTM, GRU, BiGRU) and classical time series forecasting models (ARIMA) have been implemented to forecast Apple stock returns. 
Equally important, the obtained results are compared to find the most consistent predictors and eventually the most appropriate model. The experiment results are conducted on a real dataset about Apple returns gathered from [Yahoo Finance](https://finance.yahoo.com/quote/AAPL/history?p=AAPL) for a specific period (March 2015 to March 2021). In addition, we extended it with some technical indicators for financial time series using [TA](https://github.com/bukosabino/ta) package. 

On the whole, the main contributions of this repository are:
* We analyze the time series of stock price data, given a combination of market data (Open, High, Low, Close, and Volume) and several technical indicators, to predict the stock price.
* We evaluate the effectiveness of our approach with a real data set harvested from Yahoo finance. 
* We conduct an extensive empirical analysis to choose the best set of features and hyperparameters. 
* We conduct a comparative study on the performance of DL models (LSTM, BiLSTM, GRU, and BiGRU) and the ARIMAX model on financial time series forecasting.
* Our experiment results show that BiGRU and ARIMAX are the best forecasting models for financial time series. 

## Data Set and Training Parameters

The dataset considered in the present study is Apple’s stock price time series.
The data, composed of 1521 trading days from March 17th, 2015, to March 30, 2021, is obtained from Yahoo Finance.
In order to get the best results, the deep learning models require hyperparameter tuning. These parameters are presented as the batch size, the number of epochs, and the window size.
As for the ARIMAX model, the Auto-ARIMA approach automatically finds the optimal parameters p, d, and q.

## Performance Assessment
Extensive evaluations have been presented on the performance of these models, and the results are critically analyzed. The results are shown in terms of Mean Absolute Error (MAE), Mean Absolute Percentage Error (MAPE), and Root Mean Square Error (RMSE).

## Experimental Settings
To assess the effectiveness of our approach, we executed the LSTM, GRU, BiLSTM, BiGRU, and ARIMAX models on the same training set and test set. In the same operating environment of Google Collaboratory, all experiences were conducted with one single-core hyper-threaded Xeon Processors @2.3Ghz and 12 GB of memory.

## Conclusion
As a result, BiGRU and ARIMAX models proposed in this repository performed in close manners in terms of error values. These models can reasonably predict the closing price of the following day and provide better references and insights for future investments. Moreover, these performances are achieved using the daily open, high, low, and cumulative returns of the company, denoted as F5 in the [data construction notebook](https://github.com/s0v1x/AriStocks/blob/main/Data_Construction.ipynb).

## Authors
* Conducted by: LABIAD Salah Eddine[(@s0v1x)](https://github.com/s0v1x) & ATERHI Mouad[(@AterhiM)](https://github.com/AterhiM)
* Mentored by: [Pr. KALLOUBI Fahd](https://github.com/FahdKalloubi1)
  