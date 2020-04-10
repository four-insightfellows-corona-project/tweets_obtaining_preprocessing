This repository contains Jupyter notebooks that I use to extract and preprocess tweets using tweepy. These consist of all tweets since March 1, 2020, which were published within Prospect Park in Brooklyn, New York.


The dataframe geotweets_labeled.pkl has been hand labeled up to a certain date. To update it for further hand-labeling, run tweet_getter.ipynb, then EDA.ipynb, then labeling_the_tweets.ipynb. This will provide the most recent tweets in the standard format. You can then follow the procedure embodied in labeling_the_tweets.ipynb to hand-label the most recent tweets.