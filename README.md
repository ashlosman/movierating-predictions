# movierating-predictions

We are three UCI Data Science students performing an analysis on movie rating predictions based on public opinion data from Twitter and Metacritic. This repository is being used to organize the code for our Data Science Capstone Project. 

The manual instructions to cultivate the final model and results are as follows: 

## Step 1: Vader Sentiment and Word2Vec Word Embedding Calculations

For both the twitter and metacritic data files, the respective files should be run:
- TWITTER_vader_word2vec.ipynb
  - required input files: sample_twitter.csv
  - output files: sample_twitter_vader.csv, sample_twitter_doc_reduction.csv
- METACRITIC_vader_word2vec.ipynb
  - required input files: sample_metacritic.csv
  - output files: sample_metacritic_vader.csv, sample_metacritic_doc_reduction.csv

## Step 2: Join Tables 
- regression_twitter_metacritic.ipynb
  - Run "Join Tables" section
  -  required input files: sample_twitter_vader.csv, ratings_clean.csv, sample_metacritic_vader.csv, sample_metacritic_doc_reduction.csv, sample_twitter_doc_reduction.csv

## Step 3: Build Models
- regression_twitter_metacritic.ipynb
  - Run "Modeling" section

### File Descriptions
- TWITTER_vader_word2vec.ipynb
  - This file computes the compound vader sentiment as well as the word embeddings for the twitter dataset. 

- METACRITIC_vader_word2vec.ipynb
  - This file computes the compound vader sentiment as well as the word embeddings for the metacritic dataset.

- regression_twitter_metacritic.ipynb
  - This file joins and cleans both the twitter and metacritic datasets and builds the regression models. 
- regression_twitter.ipynb
  - This file builds the regression models for the twitter dataset only.
- regression_metacritic.ipynb
  - This file builds the regression models for the metacritic dataset only. 



**NOTE ON HTML FILES:
- lasso-regression-twitter-metacritic1.html
  - Due to difficulties obtaining the entirety of the word embeddings on the full twitter dataset, the HTML file provides the output combining the numerous datasets we had to join to get the full amount of word embeddings. The updated file in the repository was completed using the sample data. 

Due to the size of the full datasets, they are unable to be uploaded to this repository. They can be found on this google drive link: https://drive.google.com/drive/folders/1XXl70YMiQ5CwJjKI-7ndIc1zhy6KCOCg?usp=sharing


