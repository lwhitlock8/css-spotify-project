This is a project in the course Computational Social Science at DTU, spring 2024. 

The aim of the project is to do webscraping at a Wikipedia page with the Coachella festival line-ups through the years (https://en.wikipedia.org/wiki/Coachella_Festival_line-ups). 
Then, the aim is to utilize these artist names to collect data and create a data set with artists that have performed at Coachella the last 24 years. This data set is created by API calls to Spotify, to gather data about the artist name, artist-ID at Spotify, genres and popularity. 
Subsequently, song and lyric data for each artist is collected, this time with API calls to MusixMatch.com. 
The data collection part of the project is carried out with libraries as Spotipy and BeautifulSoup, and it can be found in the file **data_collection.ipynb**. 

With the data set, a network of Coachella artists is created, and comprehensive network science is carried out on the network. 
For example, analysis of the relationship between the artists is performed, and the analysis also focuses on the popular genres at the festival, and at each stage, each year. 
A sentiment analysis is also performed on the lyrics of the songs of each artist, to identify possible patterns through out the 24 years that are analysed. The results are presented with histograms. 
In addition, word clouds with predominantly utilized words in the songs are presented.

Finally, a website is created with the help of a template from GitHubs Pages. 
On the website, data and results from the data analysis is presented. 
