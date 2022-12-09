# Reddit Comment Sentiment Analysis on Music Artists or Songs

This is the documentation for the CS 410 Course Project

The idea behind this program is to take reddit comments from the Music subbreddit and determine sentiment based on comments that talk about the song or artist you choose.

The program uses the reddit api to create a reddit app and then uses the API Wrapper PRAW to pull comments from the specifed subrreddit. The next steps of the program are to clean and process the word data from the comments. This is when we make use of NLTK to tokenize and stem the words. After the data is cleaned and ready to be used. We use the VADAR sentiment analyizer to determine the sentiment of the words. After the data is run through VADER we use a pandas dataframe to structure the data. 

The results of the program will provide Bar Chart showing the percentage of negative and positive words and then will produce a wordcloud that shows the most common words in the comments

 
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

from wordcloud import WordCloud

import re

# Walk through on how to setup Reddit App

The start of this article has a good walkthrough on how to set up the reddit app and gain the credentials
https://medium.com/geekculture/creating-a-reddit-bot-with-python-and-praw-185387248a22

# Utilized tutorials and walk throughs
The following are links to documentation and tutorials used to learn how to use Python, PRAW, NLTK, VADAR

1. https://levelup.gitconnected.com/reddit-sentiment-analysis-with-python-c13062b862f6 Credit to this site that helped understand how to perform this work.
2. https://praw.readthedocs.io/en/stable/getting_started/quick_start.html
3. https://www.nltk.org/
