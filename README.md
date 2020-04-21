# NLP-Earning-Transcripts

NLP 7641 Final Project: Predicting Research Analysts' Ratings with Earning Transcripts

For this project, we analyze 6400 earnings transcripts that were webscraped from motleyfool.com. Our goal is to predict how research analysts will react to these transcripts. We measure analysts reaction with their corresponding buy/hold/sell reccomendation (1-5 scale). We find that a w2vec model with 500 dimensions, weighted by tf-idf is the best representation of each transcript. We feed this into a neural network and achieve a 70% accuracy and 70% F1 score.


!pip install -r requirements.txt
https://www.dropbox.com/sh/ei6yjwlhwvr9m1w/AACJIAKDpLstyXWoTYuj1Op4a?dl=0
