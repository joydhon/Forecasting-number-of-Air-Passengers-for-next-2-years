# Forecasting-number-of-Air-Passengers-for-next-2-years

## 𝐏𝐚𝐫𝐭 𝟏: 𝐃𝐚𝐭𝐚 𝐄𝐱𝐩𝐥𝐨𝐫𝐚𝐭𝐢𝐨𝐧 𝐚𝐧𝐝 𝐏𝐫𝐞𝐩𝐫𝐨𝐜𝐞𝐬𝐬𝐢𝐧𝐠
$ Identified a clear increasing trend and seasonality in the passenger dataset.
$ Detected missing values and applied forward fill method to handle them.
$ Conducted logarithmic transformation to stabilize variance and make the data more stationary.

## 𝐏𝐚𝐫𝐭 𝟐: 𝐀𝐑𝐈𝐌𝐀 𝐌𝐨𝐝𝐞𝐥 𝐅𝐢𝐭𝐭𝐢𝐧𝐠 𝐚𝐧𝐝 𝐄𝐯𝐚𝐥𝐮𝐚𝐭𝐢𝐨𝐧
$ Selected an ARIMA(1, 1, 1) model with seasonal_order=(1, 0, 1, 12) based on AIC (Akaike Information Criterion) and BIC (Bayesian Information Criterion) values.
$ The fitted ARIMA model provided reasonable statistical significance for the parameters.
### 𝐌𝐨𝐝𝐞𝐥 𝐞𝐯𝐚𝐥𝐮𝐚𝐭𝐢𝐨𝐧 𝐦𝐞𝐭𝐫𝐢𝐜𝐬:
         $ Mean Absolute Percentage Error (MAPE): 7.25%
         $ Root Mean Squared Error (RMSE): 38.11
         $ Autocorrelation Function at lag 1 (ACF1): 0.45
         $ Pearson correlation coefficient (corr) between forecasted and actual values: 0.98

## 𝐏𝐚𝐫𝐭 𝟑: 𝐅𝐨𝐫𝐞𝐜𝐚𝐬𝐭𝐢𝐧𝐠 𝐅𝐮𝐭𝐮𝐫𝐞 𝐃𝐚𝐭𝐚
$ Generated forecasts for future time periods using the fitted ARIMA model.
$ Prepared the dataset for forecasting by extending it with future dates.
$ Applied the ARIMA model to forecast passenger numbers for the future.
$ The forecasted values aligned well with the historical data trends.

## 𝐎𝐯𝐞𝐫𝐚𝐥𝐥 𝐈𝐧𝐬𝐢𝐠𝐡𝐭𝐬 𝐚𝐧𝐝 𝐂𝐨𝐧𝐜𝐥𝐮𝐬𝐢𝐨𝐧:
$ The ARIMA model successfully captured the underlying patterns in the passenger dataset, including trend and seasonality.
$ Forecasting accuracy metrics indicated a reasonably good fit of the model to the data.
$ The forecasted values can be used for future planning and decision-making, such as resource allocation and capacity management in the transportation sector.
$ Further refinements and adjustments to the model parameters may improve forecasting accuracy in future iterations.
