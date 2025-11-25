# Project: Options Trading Using Implied vs Predicted Volatility

## This project builds a simple options-trading signal by comparing:

Implied Volatility (IV): taken from the price of an at-the-money option with ~30 days to expiration.

Predicted Realized Volatility (RV): forecasted from historical data using basic ML.

## The idea:

* If IV > predicted RV, options may be overpriced → short volatility.

* If IV < predicted RV, options may be underpriced → long volatility.

I simulate these long/short volatility positions and evaluate how the strategy performs.

## Steps

* Load stock + option data

* Compute IV using Black-Scholes

* Compute historical RV

* Build ML model to predict future RV

* Generate long/short volatility signals

* Run a simple backtest
