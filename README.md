# Reddit Comment Sentiment Analysis on Music Artists or Songs

This is the documentation for the CS 410 Course Project

The idea behind this program is to take reddit comments from the Music subbreddit and determine sentiment based on comments that talk about the song or artist you choose.

The program uses the reddit api to create a reddit app and then uses the API Wrapper PRAW to pull comments from the specifed subrreddit. The next steps of the program are to clean and process the word data from the comments. This is when we make use of NLTK to tokenize and stem the words. After the data is cleaned and ready to be used. We use the VADAR sentiment analyizer to determine the sentiment of the words. After the data is run through VADER we use a pandas dataframe to structure the data. 

The results of the program will provide Bar Chart showing the percentage of negative and positive words and then will produce a wordcloud that shows the most common words in the comments
