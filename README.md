# NLP-Earning-Transcripts

NLP 7641 Final Project: Predicting Research Analysts' Ratings with Earning Transcripts

For this project, we analyze 6400 earnings transcripts that were webscraped from motleyfool.com. Our goal is to predict how research analysts will react to these transcripts. We measure analysts reaction with their corresponding buy/hold/sell reccomendation (1-5 scale). Our analyst reccomendations were obtaining from a Georgia Tech Bloomberg Terminal using an Academic License. We find that a w2vec model with 500 dimensions, weighted by tf-idf is the best representation of each transcript. We feed this into a neural network and achieve a 70% accuracy and 70% F1 score.

To run our code you can follow the below steps:
1. Run the command '!pip install -r requirements.txt' to install all necessary packages (if not running this command in jupyter notebook, remove the "!".) 
2. If you would like to run the webscraper, the jupyter notebook file is in "WebScraping" folder
  () Make sure you download the files in the corresponding data folder (should stay in data folder) WebScraping -> data
  () Webscraping took about 40 hours on a local machine
  () The output is transcripts1.db file (data is stored on a SQLite3 db)
3. If you would like to skip webscraping, the transcripts1.db file can be downloaded at this dropbox link. The file is 690mb which is too large to host on github. https://www.dropbox.com/sh/ei6yjwlhwvr9m1w/AACJIAKDpLstyXWoTYuj1Op4a?dl=0

4. In the "Analysis" folder we have our code for our tf-idf, bag-of-words, w2vec analysis. You will need the transcripts1.db in the same directory as the analysis code you will be running.  


