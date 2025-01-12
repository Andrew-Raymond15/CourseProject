# Reddit Comment Sentiment Analysis on Music Artists or Songs

This is the documentation for the CS 410 Course Project

The idea behind this program is to take reddit comments from the Music subbreddit and determine sentiment based on comments that talk about the song or artist you choose.

The program uses the reddit api to create a reddit app and then uses the API Wrapper PRAW to pull comments from the specifed subrreddit. The next steps of the program are to clean and process the word data from the comments. This is when we make use of NLTK to tokenize and stem the words. After the data is cleaned and ready to be used. We use the VADAR sentiment analyizer to determine the sentiment of the words. After the data is run through VADER we use a pandas dataframe to structure the data. 

The results of the program will provide Bar Chart showing the percentage of negative and positive words and then will produce a wordcloud that shows the most common words in the comments

# Steps to run Jupyter Notebook

1. Open jupyter note book above
2. Install Required packages and software listed below
3. Create Reddit App Script
  
  a. https://www.reddit.com/prefs/apps/

4.Entire login information in the highlighted spot in the notebook
![image](https://user-images.githubusercontent.com/60722122/206621224-9bec03c7-6f4d-4559-aacb-732bf892e9fd.png)

5.Entire desired song or artist in cell
 ![image](https://user-images.githubusercontent.com/60722122/206621339-538dd60b-0386-4e09-87bb-2535fa378a4f.png)

6. Run Rest of cells!

7. Get analysis and visualizations!
 
# Required Packages and Downloads
 
pip install praw emoji wordcloud
 
pip install spacy

spacy download en

from IPython import display

import math

import pandas as pd

import numpy as np

import nltk

from nltk.tokenize import RegexpTokenizer

from nltk.stem import WordNetLemmatizer

from nltk.sentiment.vader import SentimentIntensityAnalyzer

import matplotlib.pyplot as plt

import seaborn as sns

import emoji

import spacy

import sys

from wordcloud import WordCloud, STOPWORDS

import re

# Walk through on how to setup Reddit App

The start of this article has a good walkthrough on how to set up the reddit app and gain the credentials
https://medium.com/geekculture/creating-a-reddit-bot-with-python-and-praw-185387248a22

# Utilized tutorials and walk throughs
The following are links to documentation and tutorials used to learn how to use Python, PRAW, NLTK, VADAR
The first link is a very helpful walkthrough that I built the base of my program off of.

1. https://levelup.gitconnected.com/reddit-sentiment-analysis-with-python-c13062b862f6 
2. https://praw.readthedocs.io/en/stable/getting_started/quick_start.html
3. https://www.nltk.org/


# Presentation and Walkthrough
https://youtu.be/9vR0RyZp2GI
