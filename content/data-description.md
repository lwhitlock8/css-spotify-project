---
title: Data description
prev: "/"
next: network-analysis
---

#### **Dataset**
Two datasets were created for our analysis: 
1. ## [Artist Dataset](https://github.com/lwhitlock8/css-spotify-project/blob/main/data/coachella_artists_full.csv)
1. ## [Raw Song Dataset](https://github.com/lwhitlock8/css-spotify-project/blob/main/data/lyrics_dataset.csv)

**1. Artist Data**
This dataset contains all of the artists that have performed at Coachella, from 1999 to 2023, which stage they performed on and information about each artist (id, music genre, followers, popularity level). We retrieved this information by scraping the Wikipedia page: “Coachella Festival Line-Ups,” and by using the Spotify API.

**2. Song Data**
This dataset contains raw lyric data sourced from the MusixMatch API. This API allows for free access to 30% of lyrics for each song with a reasonable rate limit. Due to API limits and the 30% cap on lyrics, we decided to focus only on artists that performed on the Coachella Main Stage, regardless of the year. We searched for the top 5 songs that have lyrics on MusixMatch for each artist, finding a total of 1292 songs that met the criteria.

#### **Why These Datasets?**
These datasets were chosen for a few reasons, mainly that they contain the necessary data that aligns with the goal for our analysis. We are analyzing data from Coachella since its first year in 1999 and the Wikipedia page contains all of the Coachella information needed. Combining the Coachella data with artist data from the Spotify API, we created a completed data set (for our analysis). Furthermore, we know that both our datasets contain accurate data, as it was retrieved from reliable sources, such as Wikipedia, Spotify and MusixMatch. Both datasets are also of desirable size, allowing us to conduct a thorough analysis. Lastly, the data we retrieved was accessible and available for use, another important aspect of a dataset. 

#### **Data Cleaning & Preprocessing**
The **Artist Dataset** did not need any cleaning or preprocessing. It was important that we did not clean our dataset to get rid of duplicates, because one of the main aspects of our analysis was seeing if artists performed multiple times, and seeing which stage they returned to perform on.

The artist dataset contains 2912 rows of artists, 428 KB, and has 7 variables. This includes data for every artist to perform at Coachella since its inception in 1999 including the which stage they performed on, which years they were invited, their popularity on Spotify, and their most applicable genres.

The **Song Dataset** needed some cleaning up. This included removing all punctuation, stopwords, numbers, and the commercial use copyright tag generated from the MusixMatch API. We also added a few variables from the artist dataset (artist id, artist name, genres) to make matching the datasets easier later on. The final dataset also includes two types of cleaned lyrics, one with stopwords and one without stopwords, the sentiment of the song, and the sentiment score of each song. 

The song dataset contains 1292 rows of song lyrics, 2791 KB, and has 9 variables. This dataset includes the top 5 songs (as determined by the MusixMatch API) for each artist that performed on the Main Stage of Coachella and the lyrics of each song. There is also a processed version of this dataset that includes cleaned lyrics and sentiment analysis scores.


<img src="/images/background.jpg" width="500" />
