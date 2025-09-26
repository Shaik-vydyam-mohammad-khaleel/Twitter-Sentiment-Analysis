Twitter Sentiment Analysis
A Python-based tool to analyze the sentiment of tweets related to a specific keyword or hashtag. This script fetches live tweets, processes them to determine sentiment, and visualizes the results in a pie chart.

Features
Live Data Fetching: Connects to the Twitter API to download a specified number of recent tweets.

Sentiment Classification: Utilizes TextBlob to classify each tweet into categories: Strongly Positive, Positive, Weakly Positive, Neutral, Weakly Negative, Negative, and Strongly Negative.

Data Cleaning: Includes a function to clean tweets by removing mentions, links, and special characters before analysis.

Data Visualization: Generates a matplotlib pie chart to provide an immediate visual summary of the public's reaction.

Reporting: Outputs both a general sentiment report (e.g., "Positive") and a detailed breakdown of the percentages for each category.

Technology Stack
Language: Python

Libraries:

tweepy: For accessing the Twitter API.

textblob: For performing sentiment analysis.

matplotlib: For data visualization and plotting the pie chart.

re (Regex): For cleaning tweet text.

Setup and Installation
To run this project on your local machine, follow these steps.

1. Clone the Repository

Bash

git clone <your-github-repo-url>
cd <repository-name>
2. Install Dependencies
Make sure you have Python 3 installed. Then, install the required libraries using pip.

Bash

pip install tweepy textblob matplotlib
3. Configure Twitter API Credentials
You need to have a Twitter Developer account to get API keys and access tokens.

Open the sentiment_analysis.py file in a text editor.

Find the DownloadData method.

Replace the placeholder values for consumerKey, consumerSecret, accessToken, and accessTokenSecret with your own Twitter API credentials.

Python

# authenticating
consumerKey = 'your key here'
consumerSecret = 'your key here'
accessToken = 'your key here'
accessTokenSecret = 'your key here'
How to Use
Once the setup is complete, you can run the script from your terminal.

Bash

python sentiment_analysis.py
The script will then prompt you to enter a search term and the number of tweets you wish to analyze.

Enter Keyword/Tag to search about: Python
Enter how many tweets to search: 100
After fetching and analyzing the tweets, the script will print a summary to the console and display a pie chart visualizing the sentiment distribution.
