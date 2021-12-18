# MINDS-Center-on-Knowledge-Graphs-Positions<br>
# Sentiment Analyis and Visualization on Telegram Crypto Group Data<br><br>
***The project has been implemented on jupyter notebook***<br><br>
Steps to run the project:<br>
1) Download the folder from the github repository.
2) Download Anaconda from https://www.anaconda.com/products/individual.<br>
3) Install the version of Anaconda which you downloaded, following the instructions on the download page.<br>
4) Congratulations, you have installed Jupyter Notebook. <br>
5) To run the notebook: Start Anaconda terminal and enter the command: jupyter notebook<br>
6) Navigate to the downloaded folder and open Sentiment_Analysis_Notebook.ipynb<br>
7) Find the kernel option on the menu tab and click restart and run all<br>


***Project explanation:***<br>
1) Read json data using utf8 encoding (Data downloaded from crypto group in Telegram).<br>
2) Created a dataframe for messages.<br>
3) Created a New dataframe by removing columns which are not useful.<br>
4) Created the date column by splitting the string into date and time at 'T'.<br>
5) Removedthe emojis and non ascii characters from each text message.<br>
6) Removed non English texts.<br> 
7) A new dataframe which has SHIB and DOGE words in the messages.<br>
9) Applied sentiment analysis using TextBlob library.
10) Create  a column for sentiment score and a count column to find the sum of messages per day after group by date.<br>
11) Used groupby date to find sum of messages in a day and avg sentiment per day.<br>
12) Creating a scatter plot for date vs avg sentiment. The bubble size potrays the number of messages in  a day.<br><br>

***Reason for Using TextBlob Sentiment Analysis:***<br><br>
TextBlob is a python library for Natural Language Processing (NLP). It is a simple library which supports complex analysis and operations on textual data. For lexicon-based approaches, a sentiment is defined by its semantic orientation and the intensity of each word in the sentence. This requires a pre-defined dictionary classifying negative and positive words. Generally, a text message will be represented by a bag of words. After assigning individual scores to all the words, final sentiment is calculated by some pooling operation like taking an average of all the sentiments.
TextBlob returns polarity and subjectivity of a sentence. Polarity lies between [-1,1], -1 defines a negative sentiment and 1 defines a positive sentiment. Negation words reverse the polarity. TextBlob has semantic labels that help with fine-grained analysis.
It is expected that the library returns exactly 0.0 either if the sentence didn’t contain any words that had a polarity in the NLTK training set or because TextBlob uses a weighted average sentiment score over all the words in each sample. This easily diffuses out the effect of sentences with widely varying polarities between words.

***Visualization of the number of messages per day and the average sentiment per day using the
plotly visualization library***<br><br>

We have used scatter plot to potray the avg sentiment per day and the size of the bubble indicates the number of messages. On clicking the bubble we can find the number of messages as well as the avg sentiment for that day.
![Visualization](/Visualization.png)




