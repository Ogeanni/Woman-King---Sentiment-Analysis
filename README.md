# The Woman King 
### A Twitter Sentiment Analysis by Ogechi Maryann Okafor
Link to this project article [Article](https://medium.com/@ogeann/the-woman-king-a-twitter-sentiment-analysis-a6f5f843e7c0)

The movie featured intriguing actors including Viola Davis, Lasha Lynch, John Boyega, Thuso Mbedu, Sheila Atim, Hero Fiennes Tiffin, Jimmy Odukoya, and Masali Baduza just to mention a few

Twitter being one of the most active social medial platforms was used to determine people's perceptions about the movie. I decided to mine tweets with the hashtag "womanking" for 13days using the Python module, Tweepy.
The analysis was to determine the most talked about cast, the locations where the tweets come from, and people's sentiments about the movie on Twitter.

## EXPLORATORY DATA ANALYSIS
When collected properly, without bias, and sanitized, data is fact and doesn't lie. Business is driven by insights, which also keep the sector competitively strong. Data must pass through a number of phases before insight may be gained from it. The processes are as follows;
- Data gathering
- Data cleaning
- Data processing
- Sentiment Analysis
- Data visualization
- Communication and Insights

## DATA GATHERING
Tweets for this project were mined for 13days from 18th to 30th September 2022. Python Module, Tweepy was used to extract tweets from Twitter API. Tweepy has its limitation, as it only extracts tweets that are 7 days old. Tweets were extracted and saved to a CSV file each day using the Pandas Module. config parser was used to store Twitter secret keys that only I can access because the source will be public.
I collected tweets with the hashtag "thewomanking", the time of the tweet, location, likes, and retweets of each tweet.

## DATA CLEANING
Cleaning data must be one of the daunting processes of EDA. I checked for missing values, duplicate values, and data types. I extracted 36800 tweets with 90, 090 retweets.
I named my columns for easy identification when manipulating the columns. There were so many unidentified locations in my data and Nan rows which I filled with "No location"

## DATA PROCESSING AND MANIPULATION
In other to extract the hashtags from the tweets, I used regular expression(re) to extract hashtags with the "thewomanking" to a new column.
To analyze the sentiment. The regex function was used to remove emojis, unwanted characters, punctuation, and URL.
To preprocesses the content of each tweet Natural Language Toolkit was used such as;
- Stopword - using NLTK to import stopwords(Unnecessary words)
- word_tokenze - splitting words(converting each word to a list)
- Lemmatization - used for text preprocessing but knows the context of words before processing.

## SENTIMENT ANALYSIS
Oxford dictionary defines sentiment analysis as the process of computationally identifying and categorizing opinions expressed in a piece of text, in order to determine whether the writer's attitude towards a particular topic, etc. is positive, negative, or neutral.
For this sentiment, I used a TextBlob to get the polarity of the tweets between [< 0, >= 1]. The polarity score identifies as "Positive" when text > 0, "Neutral" when text equals 0, and "Negative" when text < 0.

## DATA VISUALIZATION
For visualization and reporting. I saved my data frame to a CSV file using Pandas and exported it to Tableau for further insights.


## CONCLUSION
Due to limitation of Tweepy which only extract 7 days old. Tweets before the release of the movie was not included in this analysis.
Generally the perception of people about the movie is 56% positivie, 32% neutral and 15% negative. Also, having award winning cast in the movie contributed to it's popularity as one of the most used hashtag after #thewomanking was #violadavis.

The movie's momentum was maintained, in part, by its optimistic message. The majority of tweets come from the USA.
Thank you for reading through. I hope you found the film as entertaining as I did.
