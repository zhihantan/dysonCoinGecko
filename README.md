# Dyson Coin Gecko
Dyson Take Home Assessment (Coin Gecko Crypto)
# CryptoDataAnalyzer

CryptoDataAnalyzer is a simple Python tool designed to fetch and analyze cryptocurrency data from the CoinGecko API. It provides a wrapper around the pycoingecko library, allowing users to easily retrieve data for specific cryptocurrencies and timeframes.

## How to Use

1. Install the required package:
```python
pip install pycoingecko
```
2. Import the CryptoDataAnalyzer class into your Python script or Jupyter notebook:

```python
from CryptoDataAnalyzer import CryptoDataAnalyzer
```
3. Create an instance of the CryptoDataAnalyzer class:
```python
crypto_analyzer = CryptoDataAnalyzer()
```
4. Fetch data for the desired cryptocurrencies and timeframes:
```python
dataframe_xxx = crypto_analyzer.get_crypto_data('xxx', start_date, end_date)
```
5. Generate line plots for each cryptocurrency's prices, market cap, and total volume:
```python
dataframes = {
    'xxx': dataframe_xxx,
}
timeframe = (start_date, end_date)

crypto_analyzer.generate_line_plot_prices(dataframes, timeframe)
crypto_analyzer.generate_line_plot_market_cap(dataframes, timeframe)
crypto_analyzer.generate_line_plot_total_volume(dataframes, timeframe)
```

For additional details and usage examples, please refer to the Jupyter notebook provided in the repository.
