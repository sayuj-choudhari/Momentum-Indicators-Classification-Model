# Momentum-Indicators-Classification-Model
Option-picking model project based on classifying momentum indicators most correlated with short-term gains, finding positive expected value call-options trades

## Overview

This model was developed by testing the various momentum indicators for their correlation with a binary variable representative of whether the underlying asset gained 10% within the next 20 days. These indicators included the Stochastic Oscillator, rate of change in short/long term moving average, divergence of MACD lines, On-Balance Volume (OBV), etc. When running a bi-serial correlation model on these indicators it was identified that stronger correlations exist within the short and long term moving average (SMA, LMA), specifically an extreme rate of change values in the SMA or LMA tend to signify probable gains of 10% for the underlying asset. 

Running a Random Forest Classifier with binary output being whether a 10% gain occurred, and input being the rate of change of the SMA and LMA, the model should be able to classify trading opportunities with a ~70% accuracy. Thus, given an at-the-money call option (calculated to have an average price of 5% of the asset), the expected value of the $EV$


