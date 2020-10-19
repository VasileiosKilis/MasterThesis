# stock price prediction from historical time series and news articles

ABSTRACT
The stock market is a widely used investment scheme. Numerous companies are constantly trying
to integrate state-of-the-art computer science techniques into their strategic plans. The basic idea behind
these techniques is to fully automate the generation of predictions regarding the market’s movement. More
specifically, the attempt is to simulate the predictions that an expert in economics would suggest. The
purpose of this project is to design intelligent stock prediction models. At first, we researched three regression
problems, which were single step predictions from historical data, multi-step predictions from historical data,
and finally an autoregressive integrated moving average model (ARIMA). For the first two, we structured
our neural network models with the architecture of long short-term memory neural networks (LSTMs) and
compared the results we got with the traditional ARIMA model. Secondly, we used one of the latest neural
network techniques to perform sentiment analysis in economic news headlines. We again used LSTMs as a
classifier and also solved the problem via the traditional method of logistic regression, for comparison. Our
single-step model had a mean absolute error (MAE) of 1.75, our multi-step model had a 2.68 MAE and the
ARIMA model had a 3.76 MAE. Finally, we got a 52 percent accuracy from our sentiment analysis methods.

# GitLab repository

The files single-step prediction and multi-step prediction with LSTM describe the experiments
we did in chapter 4. These files run without any problems if you have all the modules installed.
The file fine-tune neural network hyperparameters refers again to chapter 4, and its the standard
procedure you follow to do a RandomizedSearchCV. To run this file your scikit-learn version should be
0.21.2 else the randomize search will return an error.
The file "arima project.ipynb" has the ARIMA model described in chapter 5. Furthermore, the
"final3.csv" contains all the predictions we did with ARIMA model.
The text sentiment analysis file contains the experiments we did in chapter 6.
Finally, the folder dataset contains all the datasets we used. "AAPL.csv" is the Apple stock dataset
we used to train our regression models. "Apple dataset mine.csv" is the labeled dataset with news headlines
we created. The rest are the original dataset we downloaded from Kaggle.
