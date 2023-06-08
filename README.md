# Data Science Portfolio

This repository contains a selection of my favorite personal projects that I've worked on.  Each project is written in Python using Jupyter Notebooks.  

If you like what you see here and want to know more about a particular project, chat about a work opportunity, or collaborate on something in the future, reach out to me at [rbush1127@gmail.com](rbush1127@gmail.com).

Enjoy!

## Modeling Frameworks

#### [Marketing Mix Modeling](https://github.com/rbush1127/Data-Science-Portfolio/blob/main/Marketing%20Mix%20Modeling/Marketing%20Mix%20Model%20Demo.ipynb)
In the linked notebook, you'll find my implementation of a Marketing Mix Model (MMM) framework.  The framework incorporates Ad-Stock, Diminishing Return, and Lag effect transformations.  The
framework is flexible, and allows the user to load any file they'd like with instructions on how to adapt it for updated field names and parameter ranges.  Please let me know if you find
a good use case for it!

## Personal Projects

#### [Forecasting the Price of Bitcoin with Prophet](https://github.com/rbush1127/Data-Science-Portfolio/blob/main/Cryptocurrency/BTC%20Forecast.ipynb)
Inspired by the work of a mysterious Twitter Bitcoin investor, I decided to see how accurately [$BTC](https://coinmarketcap.com/currencies/bitcoin/) could be modeled as a simple time series, and then extended the analysis to include trading volume as an exogenous variable.  I use the Yahoo Finance Python API to load the data, pandas for dataset management, SciKit-Learn for preprocessing and hyperparameter selection, and Facebook's Prophet package to forecast the price into the future.

Model hyperparameters were selected via grid search and a 10-split cross-validation for each parameter combination.  The highest accuracy was achieved on a 120-day forecast period, with an average error of ~$6600 across all 10 splits.

#### [PGA Tour Tournament Finishes](https://github.com/rbush1127/Data-Science-Portfolio/blob/main/PGA%20Tour/Model%20Tuning%20%26%20Feature%20Engineering.ipynb)
As an avid golfer and PGA Tour fan, I was curious to see how accurately I could predict the finish of each player at a given event if I knew the course being played, the tournament being held, and their recent performance.  In this project, I fit a Support Vector Machine which predicts whether a player will make the cut, and an XGBoost regressor to predict their finish relative to par.

The SVM achieved 75% accuracy and 82% precision in predicting whether a player would miss the cut.  The XGBRegressor predicted player's strokes relative to par with an average error of 5.1 strokes.

## Kaggle Competitions

#### [Challenges in Representation Learning: Facial Expression Recognition Challenge](https://github.com/rbush1127/Data-Science-Portfolio/blob/main/Kaggle%20Competitions/Facial%20Expression%20Recognition/Facial%20Expression%20Recognition.ipynb)
In this challenge, competitors are given a dataset made up of 48x48 grayscale images which can be one of seven emotions: Angry, Disgust, Fear, Happy, Sad, Surprise, or Neutral.  It's an older competition, so I was not able to submit an official entry.  However, my final model accurately classified 62.3% of images in the private test dataset, which would have been strong enough for a top-10 finish.

#### [Digit Recognizer](https://github.com/rbush1127/Data-Science-Portfolio/blob/main/Kaggle%20Competitions/Digit%20Recognition/MNIST%20Competition.ipynb)
A computer vision challenge using the famous MNIST image dataset, the Digit Recognizer challenge prompts the competitor to build a model which recognizes handwritten numerical digits between 0 and 9.  My model achieves 99.6% accuracy and was good enough to earn me a top 7% entry at the time of submission.
