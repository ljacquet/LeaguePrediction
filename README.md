# LeaguePrediction
High School Senior Project attempting to predict League of Legends ARAMS

# Data Used
To build my dataset I aquired the Champion Winrate, Player Champion Mastery, Player Rank and Player Summoner Level for every player in every game I used as data. 

This resulted in my having 40 parameters for my model.

# Data Preperation
1. winrate was not modified
2. The ranks of the users was changed so that it was a percent of the total rank in the game
3. Mastery was heavily skewed so I took the log of the z-score to normalize it
4. The user levels was a percent of the total. Same as with the rank.

# Conclusions
I was able to get a 65% accuracy using my own Keras model and a 68% accuracy using a sklearn linear SVC. Interestingly enough the model only takes one epoc for the model to plateau. In the future I would want to gather more data however the amount of time it takes to gather large amounts of data from the Riot API makes it less worthwhile.
