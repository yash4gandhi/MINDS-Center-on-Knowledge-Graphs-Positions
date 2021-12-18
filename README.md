# MINDS-Center-on-Knowledge-Graphs-Positions<br>
**The project has been implemented on jupyter notebook**<br><br>
Steps to run the project:<br>
1) Download the folder from the github repository.
2) Download Anaconda from https://www.anaconda.com/products/individual.<br>
3) Install the version of Anaconda which you downloaded, following the instructions on the download page.<br>
4) Congratulations, you have installed Jupyter Notebook. <br>
5) To run the notebook: Start Anaconda terminal and enter the command: jupyter notebook<br>
6) Navigate to the downloaded folder and open Sentiment_Analysis_Notebook.ipynb<br>
7) Find the kernel option on the menu tab and click restart and run all<br>


**Project explanation:**<br>
1) Read json data using utf8 encoding.<br>
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

**Reason for Using TextBlob Sentiment Analysis:**<br>

**Visualization of the number of messages per day and the average sentiment per day using the
plotly visualization library**<br>

We have used scatter plot to potray the avg sentiment per day and the size of the bubble indicates the number of messages. On clicking the bubble we can find the number of messages as well as the avg sentiment for that day




