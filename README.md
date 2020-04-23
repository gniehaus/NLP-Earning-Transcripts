# NLP-Earning-Transcripts

NLP 7641 Final Project: Predicting Research Analysts' Ratings with Earning Transcripts

For this project, we analyze 6400 earnings transcripts that were webscraped from motleyfool.com. Our goal is to predict how research analysts will react to these transcripts. We measure analysts reaction with their corresponding buy/hold/sell reccomendation (1-5 scale). Our analyst reccomendations were obtained from a Georgia Tech Bloomberg Terminal using an Academic License. We find that a w2vec model with 500 dimensions, weighted by tf-idf is the best representation of each transcript. We feed this into a neural network and achieve a 70% accuracy and 65% F1 score.

We have listed some prior work and motivating examples in our "research_papers" folder.

To run our code you can follow the below steps:
1. Run the command '!pip install -r requirements.txt' to install all necessary packages (if not running this command in jupyter notebook, remove the "!".) 

2. If you would like to run the webscraper, the jupyter notebook file is in "WebScraping" folder

  2a Make sure you download the files in the corresponding data folder (should stay in data folder) WebScraping -> data

  2b Webscraping took around 40 hours on a local machine

  2c The output is transcripts1.db file (data is stored on a SQLite3 db)

3. If you would like to skip webscraping, the transcripts1.db file can be downloaded at this dropbox link. The file is 690mb which is too large to host on github. https://www.dropbox.com/sh/cwn434x1y6ra2m2/AABZW8-nBJLGhxTN2LyMNsdNa?dl=0

4. In the "Analysis" folder we have our code for our tf-idf, bag-of-words, and w2vec analysis. You will need the transcripts1.db in the same directory as any code you choose to run.  

Project Team: Michael Hayes, Grayson Niehaus, Frank Whitesell
