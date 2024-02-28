# ARIMA_Prophet_LSTM_TimeSeries

In this notebook, we will use ARIMA, Prophet, and LSTM to predict daily minimum temperatures. Here are the main ideas for the three models:

- ARIMA Model: First, check if the time series is stationary by plotting and using the ADF test. If it's non-stationary, apply differencing. The 'd' in ARIMA represents the number of differencing needed. Afterward, use ACF and PACF plots to determine the 'p' and 'q' terms in ARIMA. An easier approach is to employ auto ARIMA.

- Prophet: This model requires only two parameters: 'ds' (representing time) and 'y' (the minimum temperatures). There's no need to check for stationarity, as Prophet can adeptly handle seasonal and trend effects.

- LSTM: This neural network uses a gated architecture to manage information over long sequences, making it well-suited for time series prediction.