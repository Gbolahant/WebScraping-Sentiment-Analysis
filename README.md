# Far From Home Twitter Scrape & Sentiment Anaylsis

----
## Introduction
This project is a web scraper that collects data on the "Far from Home" netflix series from Twitter using the hashtag (#farfromhomenetflix, #FarFromHome) & the keyword search 'FarFromHome , performs sentiment analysis on the data using the TextBlob and VADER libraries, and scrapes Google Trends data using the pytrends library. The collected data is processed using lemmatization and tokenization techniques, and is stored in a CSV file for easy analysis and manipulation.

----
## Requirements
This project requires the following libraries and tools:

* Python 3.8 or higher
* Jupyter notebook
* snscraper
* TextBlob
* VADER
* NLTK
* pytrends  

----
## Setup
To set up and run this project, follow these steps:

1. Install Python 3.8 or higher on your machine.
2. Install Jupyter notebook on your machine
3. Install the required libraries by running the following command:

```bash
!pip install snscrape
!pip install pytrends
import nltk
!pip install vaderSentiment
import pandas as pd
import snscrape.modules.twitter as sntwitter
import re, string, unicodedata
```

4. Download or clone the repository from GitHub.
5. Navigate to the project directory and open FarfromhomeTweetsScrape-.ipynb.

----
## Usage
To scrape tweets about "Far From Home" and perform sentiment analysis and search trend analysis, Click on the .ipynb file to open it
You can then run the code cells by clicking on them and pressing Shift+Enter

This will create a new CSV file, 'Farfromhome.csv', in the project directory containing the scraped tweet and search trend data. The CSV file will have the following structure:

![image](https://user-images.githubusercontent.com/109844505/210386148-95c32f55-21e9-4ecc-8b8c-9d522f5f90fe.png)

----
## Customization
The following options can be modified in the FarfromhomeTweetsScrape-.ipynb file to customize the web scraping and sentiment analysis process:

* query : The keyword that will be searched on twitter and time frame.
* limit : The maximum number of tweets to scrape and analyze.
* Output file: The name of the output CSV file.

----
## Troubleshooting
If you encounter any issues while running the web scraper, check the following:

* Make sure you have installed all required libraries and tools.
* Make sure you have added your Twitter API key and secret to the scraper.py file.
* If the script is unable to access the Twitter API, try checking your internet connection and ensuring that your firewall is not blocking the script's access.
* run this code
```bash
nltk.download('wordnet')

nltk.download('punkt')

nltk.download('averaged_perceptron_tagger')

nltk.download('stopwords')
```
