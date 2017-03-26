# Employment of Recurrent and Feedforward Neural Networks to Capture Equity Memory and Anticipate Momentum Mean Reversions
There has been much development on the usage of supervised learning to forecast financial time series by using various feature combinations of lagged price and technical indicators. Most prominently, research has applied high-dimensional support vector classifiers and feedforward neural networks trained with genetic algorithms or gradient descent. However, using such near-sighted algorithms fails to capture the full memory retention of equities. 

This study employs a long short-term memory (LSTM) structured recurrent neural network to effectively anticipate mean reversions by learning the full memory span of financial time series. The LSTM algorithm is evaluated against a feedforward network where time lags are manually selected for input based off observations of various conditional distributions of indicators, and the network is train via stochastic gradient descent and boosting. 

In both cases, we target the z-scores of momentum indicators for input and minimize model exposure to external factors by trading equities with minimal volatility and low correlation to sector exchange-traded funds (ETF). The outputs are given as predicted next day returns and positions are acquired using the long-short equity framework. The strategies are backtested using the Zipline platform. (Experiment not complete)
