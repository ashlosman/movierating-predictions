# movierating-predictions

We are three UCI Data Science students performing an analysis on movie rating predictions based on public opinion data from Twitter and Metacritic. This repository is being used to organize the code for our Data Science Capstone Project. 

__Disclaimer__: The csv files are a much smaller subset of our real dataset in interest of saving space and runtime for word2vec calculations. 

## Python Files:
|Python File| Functionality |
|---------------|---------------|
| METACRITIC_vader_word2vec.ipynb| Calculates Sentiment and Word Embeddings for Metacritic Data |
| TWITTER_vader_word2vec.ipynb | Calculates Sentiment and Word Embeddings for Twitter Data | 
| regression_metacritic.ipynb | Calculates LASSO and Linear Regression for Metacritic Data |
| regression_twitter.ipynb | Calculates LASSO and Linear Regression for Twitter Data | 
| regression_twitter_metacritic.ipynb | Calculates LASSO and Linear Regression for Metacritic and Twitter Data |

## CSV Files:
| CSV File | Functionality |
|----------|---------------|
| ratings_clean.csv | imDb ratings |
| sample_metacritic.csv | sample version of our metacritic data | 
| sample_metacritic_doc_reduction.csv | word2vec calculations for sample metacritic data | 
| sample_metacritic_vader.csv | sample metacritic vader sentiments | 
| sample_twitter.csv | sample version of our tweet data | 
| sample_twitter_doc_reduction.csv | word2vec calculations for sample twitter data | 
| sample_twitter_vader.csv | sample twitter vader sentiments | 

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
  - required input files: sample_twitter_vader.csv, ratings_clean.csv, sample_metacritic_vader.csv, sample_metacritic_doc_reduction.csv, sample_twitter_doc_reduction.csv

## Step 3: Build Models
- regression_twitter_metacritic.ipynb
  - Run "Modeling" section


**NOTE ON HTML FILES:
- regression_twitter_metacritic.html
  - Due to difficulties obtaining the entirety of the word embeddings on the full twitter dataset, the HTML file provides the output combining the numerous datasets we had to join to get the full amount of word embeddings. The updated file in the repository was completed using the sample data. 

Due to the size of the full datasets, they are unable to be uploaded to this repository. They can be found on this google drive link: https://drive.google.com/drive/folders/1XXl70YMiQ5CwJjKI-7ndIc1zhy6KCOCg?usp=sharing


