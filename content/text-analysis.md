---
title: Text analysis
prev: network-analysis
---

The text processing in this project includes wordclouds and analysis the genres for each of the ten Coachella stages/tents. This is done with the Python package "Wordcloud", to visualize the genres for each tent to identify any trends.

### **Sentiment Analysis**
In addition, text analysis on the lyrics was implemented. This was implemented by  analyzing the sentiment scores from the lyrics. This lyrics analysis only regards the artists from the main stage, and this restriction was made due to time limitation. 

It is important to note that all songs in the dataset come from performers that performed on the Main Stage of Coachella, so we cannot draw any conclusions on the festival as a whole, just the Main Stage. This is simply a limitation of the amount of textual data we could collect without a subscription to any lyric API.

#### **Sentiment Analysis Results**
Histograms were computed, an example is vizualized below. 

![](/images/Histogram.png)

The histogram shows the total sentiment scores of every song in the dataset for the corresponding year. A positive score means a positive sentiment and a negative score means a negative sentiment. We can see that there is a slight majority of songs that have a positive sentiment and the plot roughly follows a normal distribution. We expected songs to have more extreme sentiments, that is, there would be more songs that have large positive values or large negative values. Instead, it seems that most songs have relatively neutral sentiments, with few having strong positive or negative sentiments.

### **Lyrics Cloud Analysis**
In addition to sentiment analysis, we wanted to generate word clouds to identify trends in lyrics in Main Stage performances. Below you can find word clouds for each year of the festival and all the way down, you will find a word cloud for all 22 years of the festival. An exmple of a word cloud is vizualized below. 

![](/images/Artist_graph.png)

A few trend were indentified in the wordclouds created. Firstly, there are clearly groups of associated words that appear frequently, such as the "love song" group. This includes words such as: love, baby, babe, sexy, heart, etc. and could also include helper words such as: get, got, or tonight. There is also the appearance of other languages, mainly Spanish. It is very easy to tell which years included hispanic performers due to the appearance of que, el, la and other Spanish stopwords that were not removed by the English filter. 

Overall, there does not seem to be significant differences between the word clouds. It is difficult to spot trends in these word clouds as often the most interesting words appear only once while words that are common among traditional pop themes (ex: love songs) dominate the word clouds. This is not to say that the years are all the same but there are not many standout years.