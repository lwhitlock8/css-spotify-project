---
title: Data description
prev: "/"
next: network-analysis
---
![](/images/background.jpg)

For this analysis, we gathered data from three sources: 
the Wikipedia page: “Coachella Festival Line-Ups,” the Spotify API and the MusixMatch API. With this, we created two datasets, for our artist data and for our song data. 

**1.  Artist Data**
- Contains all of the artists that have performed at Coachella, from 1999 to 2023.
- Contains information on which stage they performed on.
- Artist variables: id, music genre, followers, popularity level.

In order to retrieve information about each year's Coachella lineup, we scraped the wikipedia page's data.

**2.   Song Data**
- Contains lyric data
- Each row of data includes: song name, song ID, the first 30% of each song’s lyrics.\
From the Artist Dataset, we retrieved all the artists that performed on the main stage (the largest/most famous stage), and used the Musix Match API to retrieve the lyrics of each artist’s top 5 most popular songs.



These two datasets contain the information we needed to conduct our network & text analysis. 

