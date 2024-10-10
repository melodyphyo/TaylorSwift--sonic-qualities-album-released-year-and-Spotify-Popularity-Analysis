 ![image](https://github.com/user-attachments/assets/483da596-45d9-47d6-bb1f-aa242f5c6ef2)

# Introduction

As a dedicated fan of Taylor Swift, I am inspired to explore and analyze her remarkable career using data analytics. For my data analyst portfolio, I have chosen to work with the Taylor Swift Spotify dataset sourced from Kaggle.

# Guiding Question
As a Data Analyst, guiding question for this project is “How do the sonic qualities of Songs from Taylor Swift’s albums and time line of her career affect their popularity?”

The metrics I care for this question are “popularity”, “acousticness”, “danceability”, and “liveness”. These metrics are measured, collected, and provided by “Spotify for Developers,” and here are their definitions:

* Popularity — calculated by Spotify’s algorithm, is mostly based on the number of plays and how recent those plays are. Its value will be between 0–100, with 100 being the most popular.
* Acousticness — “A confidence measure from 0.0 to 1.0 of whether the track is acoustic. 1.0 represents high confidence the track is acoustic.”
* Danceability — “Danceability describes how suitable a track is for dancing based on a combination of musical elements including tempo, rhythm stability, beat strength, and overall regularity. A value of 0.0 is least danceable and 1.0 is most danceable.”.
* Liveness — determines the likelihood of a song being performed live by measuring if an audience is detected in the track. The closer to 1.0, the more likely the song is recorded live.
By incorporating various metrics from Spotify, I included the release date in my analysis.

# Road Map for Analysis
I conducted this data analysis on Taylor Swift’s Spotify data by following a typical data analysis framework: Prepare, Process, Analysis and Share.

## Prepare and Process
### Data

* Data is stored in a CSV file
* Data was pulled from a dataset on Kaggle (Kindly take note that the data was pulled on Sep 2024)
### Data Cleaning
* Fortunately, the data was mostly clean and required minimal cleaning. I performed the data cleaning in** _Jupyter Notebook using Python and its Data Science Libraries (Pandas, Matplotlib, Seaborn)._**

* Deleted unnecessary columns for this analysis, such as uri, Unnamed: 0, and id.
* Adjusted data types where necessary.
* Created a new column for the release year, extracted from the release date.
* During data cleaning, I made sure to remove any song titles containing the string “voice memo” to ensure accurate analysis for identifying the most and least popular songs from each album, as these are not actual songs.

## Explotary Analysis
### Popularity of Track number 13 from Each Album
“We Swifties are obsessed with the number 13, as it’s Taylor Swift’s lucky number. So, I’m eager to take a look at the popularity of track number 13 from each of her albums. I mean, why not?”

![track-no13-popularity](https://github.com/user-attachments/assets/d864fb9d-1e78-4483-8b5d-6c84a3bdf246)


The x-axis lists the song names, while the y-axis represents their popularity scores, ranging from around 30 to 90.


**Key Observation from above line chart:**

* Highest Popularity: “I can do with a Broken Heart” stands out with the highest popularity score, close to 90.
(This track hails from Taylor’s latest album, “TTPD.” After the album’s release, Taylor included the TTPD era in her Eras Tour setlist. The performance of this song during the tour has been nothing short of spectacular, quickly becoming a fan favorite.)
* Notable Highs: Songs like “Clean (Taylor’s Version)” and “I Can Do It With a Broken Heart” have relatively high scores, around 70–80.
* 
### Taylor Swift’s Career Popularity by Album Release Year

![popularity of taylor swift career upon the album release year](https://github.com/user-attachments/assets/201b3454-e631-4dc0-a0a1-60384ebae203)


The bar chart tracks Taylor Swift’s career popularity based on her album release years, spanning from 2006 to 2024. Each bar’s height represents the popularity level for that specific year.

**Key observations from the chart:**

* 2006: Her debut year shows a solid start with popularity around 65.
* 2008: There’s a noticeable dip to around 55, possibly reflecting a period of lower impact or competition.
* 2010: Popularity rises to approximately 70, indicating a rebound.
* 2012: A decline is observed with popularity dipping to around 60.
* 2014 onwards: There’s a general upward trend, peaking significantly in 2019 with a popularity score of around 90.
* 2017 to 2024: Popularity remains high, fluctuating between 80 and 90, showing consistent audience engagement.
The lowest popularity is observed in 2008, while the highest is in 2019, marking key points in her career. Overall, the chart vividly illustrates the fluctuations and trends in Taylor Swift’s popularity over nearly two decades, highlighting her significant peaks and periods of consistency.

### Most Popular Song from Each Album

![most-popular-song](https://github.com/user-attachments/assets/22c9b5a4-8fe6-45d9-bbcd-ec9aa1ac80d6)


The horizontal bar chart displays the popularity of the most popular song from each of Taylor Swift’s albums. The x-axis represents the popularity score, while the y-axis lists the song titles. Each bar indicates the popularity level of a song, with longer bars representing higher popularity.

**Key observations:**

* Top Songs: “Cruel Summer” leads the pack with the highest popularity score, followed closely by “Fortnight (feat. Post Malone)” and “Anti-Hero.”
* High Popularity: Songs like “cardigan,” “You Belong With Me (Taylor’s Version),” and “Blank Space” also exhibit high popularity scores.
* Middle Range: Songs such as “Willow,” “Wildest Dreams,” and “right where you left me — bonus track” fall into a middle popularity range.
* Lower Popularity: “Beautiful Eyes — Live From Clear Channel Stripped 2008” and “Love Story” have lower popularity scores among the listed songs.
The chart effectively showcases the most popular songs from Taylor Swift’s various albums, highlighting her hits over the years and providing a clear visual comparison of her top tracks’ popularity.

### Least Popular Song from Each Album

![lease-popular-song](https://github.com/user-attachments/assets/a6088723-c6e0-4a92-bae9-a859b93de8a0)


The bar chart showcases the least popular songs from each of Taylor Swift’s albums. The x-axis represents the popularity scores, while the y-axis lists the song titles.

**Key Observations:**

* Lowest Popularity: The song “Change” appears twice, indicating it is the least popular song in two different contexts — one from a live performance in 2008 and another as a regular track.
* Moderate Popularity: Songs like “Back to December,” “Treacherous — Original Demo Recording,” and “Sad Beautiful Tragic” fall into a moderate popularity range.
* Higher Popularity Among Least Popular: “Robin,” “So It Goes…,” and “I Can Fix Him (No Really I Can)” are among the least popular but still have relatively higher popularity scores compared to the other least popular songs.

### Acousticness and Popularity

![scatter-plot_acou-pop](https://github.com/user-attachments/assets/8d088ff8-6f6a-47fa-b5f5-655a258c1bd9)


The scatter plot illustrates the relationship between the popularity (x-axis) and acousticness (y-axis) of various songs from Taylor Swift’s albums. Each point represents a song, with colors differentiating albums.

The trend line suggests a slight positive correlation between popularity and acousticness, although this relationship isn’t strong. Albums like “Midnights” and “evermore” show higher acousticness and popularity, suggesting listener preference for these qualities in Taylor Swift’s recent work.

### Danceability and Popularity

![scatter-plot_dance-pop](https://github.com/user-attachments/assets/0ac63147-fe5d-4bc4-8372-0fe28f3c1409)


The scatter plot explores the relationship between the popularity (x-axis) and danceability (y-axis) of Taylor Swift’s songs from various albums, color-coded by album.

The chart highlights a slight positive relationship between a song’s danceability and its popularity. This insight underscores that while danceability can contribute to a song’s popularity, it is not the sole factor.

There’s a broad distribution in danceability scores across different popularity levels, indicating that while there’s a slight trend, not all popular songs are highly danceable.

### Liveness and Popularity

![scatter-plot_live-pop](https://github.com/user-attachments/assets/b61327b8-0689-456f-bb3e-a9a9cf713ae6)


The scatter plot shows the relationship between the popularity of Taylor Swift’s songs (x-axis) and their liveness (y-axis). Each dot represents a song, color-coded by album.

The trend line indicates a slight negative correlation between popularity and liveness. This suggests that more popular songs tend to have lower liveness.

### Released Year and Popularity

![scatter-plot_year-pop](https://github.com/user-attachments/assets/9ef7dbdf-e22f-4604-be55-b4fb56e17295)


This scatter plot explores the relationship between the popularity of songs and their release year, with each dot representing an album and color-coded accordingly. The x-axis represents the popularity of songs, ranging from 30 to 90, while the y-axis represents their release year, spanning from 2005 to 2025.

The trend line indicates a positive correlation between the release year and popularity. This means that more recent albums tend to be more popular. The clustering of dots suggests that recent albums, such as those released from 2020 onwards, generally have higher popularity ratings.

Notably, albums like “Midnights,” “evermore,” and “folklore” are prominently represented, showing they have numerous songs in the dataset. These albums, released in the recent years, align with the overall positive trend, indicating their strong performance in terms of popularity.

One point in the chart represents the year 2025, despite the dataset not containing this year. This suggests a possible data entry error or an outlier. Removing this outlier would ensure a more accurate representation.

In summary, the scatter plot underscores the trend that newer albums tend to be more popular, reflecting evolving listener preferences and the impact of recent releases.

## Conclusion
We observed that while there are slight positive correlations between popularity and both acousticness and danceability, these trends are not particularly strong. Release date is the biggest key factor when it comes to the popularity of a Taylor Swift release. Additionally, newer albums generally display higher popularity, underscoring the artist’s evolving resonance with her audience.

# Share
View the GitHub for this analysis here (link)

You can read the article for this analysis [here] (https://medium.com/@melodyphyo/taylor-swift-spotify-popularity-analysis-b060bb83ce82) (here)
