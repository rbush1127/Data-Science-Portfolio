# Data Science Portfolio

This repository contains a selection of my favorite personal projects that I've worked on.  Each project is written in Python using Jupyter Notebooks.  

If you like what you see here and want to know more about a particular project, chat about a work opportunity, or collaborate on something in the future, reach out to me at [rbush1127@gmail.com](rbush1127@gmail.com).

Enjoy!


## [Forecasting the Price of Bitcoin with Prophet](https://github.com/rbush1127/Data-Science-Portfolio/blob/main/Cryptocurrency/BTC%20Forecast.ipynb)
Inspired by the work of a mysterious Twitter Bitcoin investor, I decided to see how accurately [$BTC](https://coinmarketcap.com/currencies/bitcoin/) could be modeled as a simple time series, and then extended the analysis to include trading volume as an exogenous variable.  I use the Yahoo Finance Python API to load the data, pandas for dataset management, SciKit-Learn for preprocessing and hyperparameter selection, and Facebook's Prophet package to forecast the price into the future.

Model hyperparameters were selected via grid search and a 10-split cross-validation for each parameter combination.  The highest accuracy was achieved on a 120-day forecast period, with a cross-validated error of ~$6600 across each 120-day time period.

## [PGA Tour Tournament Finishes](https://github.com/rbush1127/Data-Science-Portfolio/blob/main/PGA%20Tour/Model%20Tuning%20%26%20Feature%20Engineering.ipynb)
As an avid golfer and PGA Tour fan, I was curious to see how accurately I could predict the finish of each player at a given event if I knew the course being played, the tournament being held, and their recent performance.  In this project, I fit a Support Vector Machine which predicts whether a player will make the cut, and an XGBoost regressor to predict their finish relative to par.

The SVM achieved 75% accuracy and 82% precision in predicting whether a player would miss the cut, and the XGBRegressor predicted player's strokes relative to par with an average error of 5.1 strokes.
