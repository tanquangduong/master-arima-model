# master-arima-model
Master ARIMA model for forcasting


## ✅ Setup Env
- Create Python environment\
`conda create -n env_name python=3.10`\
`conda activate env_name`
- Create Python environment\
`pip install -r .\path_to_requirements\requirements.txt`

## Time series
- Properties:
  - Trend: positive/negative trend is a line the generally slope up/down
  - Seasionality: patterns that repeat at regular intervals
  - Cyclicality: repeating pattern but no fixed period
  - Noise: the current value is not relevant to value that came before
  - Stationary: 
    - Distribution of the data doesn't change with time. 
    - The variance is constant 
    - Autocorrelation is constant
- Test non-stationary: Dicky-Fuller test
  - Tests for trend non-stationarity
  - Null hypothesis is that time-series is non-stationary
  - Oth element is test statistic: More negative means more likely to be stationary
  - 1st element is p-value: if p-value is small -> reject null hypothesis. Reject non-stationary
- Time series models
  - AR: Auto Regressive model
  - MA: Moving Average model
  - ARMA: AR + MA