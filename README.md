This repository contains Jupyter notebooks that I use to extract and preprocess tweets using tweepy. These consist of all tweets since March 1, 2020, which were published within Prospect Park in Brooklyn, New York.


The dataframe geotweets_labeled.pkl has been hand labeled up to a certain date. To update it for further hand-labeling, run tweet_getter.ipynb, then EDA.ipynb, then labeling_the_tweets.ipynb. This will provide the most recent tweets in the standard format. You can then follow the procedure embodied in labeling_the_tweets.ipynb to hand-label the most recent tweets.

The dataframe geotweets_labeled_binned.pkl is a de-indexed version which contains a time-bin column, assigning each tweet to a bin of 05, 20, 35, or 50 minutes past the hour. 


geotweets_labeled_binned.pkl contains the following columns: 

date - the exact date the tweet was published, in EST

text - the text contents of the tweet, including URLs leading to websites or photos

username - username of tweeter

day_of_week - day of the week

hour - hour that the tweet was published

safe - whether the tweet indicates that it was unsafe (0) or safe (1) to go to the park due to considerations of crowding and social distancing.  

binned_date - a time-bin column, assigning each tweet to a bin of 05, 20, 35, or 50 minutes past the hour. 
