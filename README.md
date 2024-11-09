# Exploratory Data Analysis on Spotify 2023 Dataset
## Course: ECE 2112 - Advanced Computer Programming and Algorithms
#### University of Santo Tomas, Electronics Engineering Department
---
# Introduction
In this deliverable, you will perform an exploratory data analysis (EDA) on a dataset containing information about popular tracks on Most Streamed Spotify Songs 2023 (https://www.kaggle.com/datasets/nelgiriyewithana/top-spotify-songs-2023Links to an external site.). This task aims to analyze, visualize, and interpret the data to extract meaningful insights.

## Summary of Problems
### Overview of Dataset:
- How many rows and columns does the dataset contain?
  - There are 953 rows and 24 columns in the dataset.
- What are the data types of each column? Are there any missing values?
  - The dataset includes a combination of integers and strings. Examples of string data types are track name and artist name, while integer data types include artist count, released year, and more. There are some missing values in_shazam_charts and key.
 
### Basic Descriptive Statistics:
- What are the mean, median, and standard deviation of the streams column?
  - ![image](https://github.com/user-attachments/assets/4c70bb1f-8ee4-4fc5-81ae-337218efb70c)
  - The mean number of streams is 514,137,424, with a median of 290,530,915 streams and a standard deviation of 566,856,949 streams.
- What is the distribution of released_year and artist_count? Are there any noticeable trends or outliers?
  - ![image](https://github.com/user-attachments/assets/2e78ebed-6813-4837-9086-5fa901b268dc)
  - The distribution of release years shows an increasing trend over time. From the early 1930s to the 1990s, there were fewer releases, likely due to the limitations of technology at the time. By 2023, releases have reached a peak, with over 400 tracks released.
  - The distribution of artist counts shows a declining trend, with the majority of tracks featuring only one artist—over 1,000 tracks fall into this category. The number of tracks decreases as the artist count increases.

### Top Performers:
- Which track has the highest number of streams? Display the top 5 most streamed tracks.
  - ![image](https://github.com/user-attachments/assets/f161dc9a-de04-4126-80e1-5efcbbfc914b)
  - The track with the highest number of streams is "Blinding Lights" by The Weeknd, with 3,703,895,074 streams. Following it are "Shape of You" by Ed Sheeran, "Someone You Loved" by Lewis Capaldi, "Dance Monkey" by Tones and I, and "Sunflower" by Post Malone and Swae Lee.
- Who are the top 5 most frequent artists based on the number of tracks in the dataset?
  - ![image](https://github.com/user-attachments/assets/e790cf75-3156-41ef-86db-01ccc5dae373)
  - The top five most frequent artists are led by Taylor Swift, with 34 tracks, followed by The Weeknd, Bad Bunny, SZA, and Harry Styles.
 
### Temporal Trends:
- Analyze the trends in the number of tracks released over time. Plot the number of tracks released per year.
  - ![image](https://github.com/user-attachments/assets/b2113155-2558-4496-8587-4328d43597ce)
  - Over time, the number of track releases has steadily increased, reaching a peak in 2022 with over 400 tracks released.
- Does the number of tracks released per month follow any noticeable patterns? Which month sees the most releases?
  - ![image](https://github.com/user-attachments/assets/f3c51723-d479-402b-a40d-482c4c62cdf1)
  - January and May have the highest number of track releases, likely due to the start of the year and the beginning of summer, when many people, especially students, are more inclined to listen to music.

### Genre and Music Characteristics
- Examine the correlation between streams and musical attributes like bpm, danceability_%, and energy_%. Which attributes seem to influence streams the most?
  - ![image](https://github.com/user-attachments/assets/724d73b2-308a-48d5-9198-2da3a15b37a4)
  - There is no clear correlation between streams and musical attributes like BPM, danceability, and energy. Tracks with a wide range of BPM values, from around 60 to 200, show varied stream counts, suggesting that BPM may not significantly influence a track's popularity. Danceability shows a slightly stronger relation with streams than the other attributes, but still lacks a clear correlation. Similarly, the energy plot reveals that streams are distributed across all energy levels, indicating no strong relationship between energy and streams.
- Is there a correlation between danceability_% and energy_%? How about valence_% and acousticness_%?
  - ![image](https://github.com/user-attachments/assets/f29ab546-18b4-4ca4-94df-33ada4486e9c)
  - There appears to be a positive correlation between danceability and energy, as the scatterplot shows an increasing trend. This suggests that songs with higher danceability tend to have more energy, which aligns with the idea that danceable tracks are often fast-paced and upbeat. Valence and acousticness do not seem to have a clear correlation, as the scatterplot does not show any noticeable pattern between the two.
### Platform Popularity
- How do the numbers of tracks in spotify_playlists, spotify_charts, and apple_playlists compare? Which platform seems to favor the most popular tracks?
  - ![image](https://github.com/user-attachments/assets/4f718730-0298-4e71-942c-77fb987dcd52)
  - The Spotify playlists contain the highest number of tracks compared to both Apple playlists and the Spotify Charts. This is likely due to the higher number of streams on Spotify, which results in Spotify playlists often favoring a larger selection of tracks compared to the other platforms.

### Advanced Analysis
- Based on the streams data, can you identify any patterns among tracks with the same key or mode (Major vs. Minor)?
  - ![image](https://github.com/user-attachments/assets/d186c3ea-7e5b-4b9c-a27b-01c24fc8b295)
  - Songs in major keys tend to dominate mainstream charts and playlists. However, minor key songs can also achieve significant popularity, particularly in genres that emphasize emotional depth and expression.
- Do certain genres or artists consistently appear in more playlists or charts? Perform an analysis to compare the most frequently appearing artists in playlists or charts.
  - ![image](https://github.com/user-attachments/assets/48981712-5d68-4bbc-8b7c-d1d61ea5c08c)
  - It is not entirely consistent, as the chart_count does not always correlate with the playlist_count. For example, Taylor Swift ranks second behind The Weeknd in terms of total tracks, yet she has significantly more chart appearances. This indicates that while both playlist and chart counts reflect an artist's popularity, they do not always align in terms of their overall representation.
 
---
## How can this be related to real-life?
Python has many applications in real-life especially now that the world revolves around the use of technology. Some of the top real-life applications of Python are:
- Web Development
- Game Development
- Artificial Intelligence
- Data Science
- Audio and Visual or Image Processing

## Best Practices To Do When Coding
When coding, it is best to do practices that would help you efficiently write codes. The top 5 best practices when coding in Python are:
- Usage of descriptive variable names.
- Usage of variables for constants.
- Leaving comments and taking documentation.
- Usage of whitespace.
- Be consistent with the codes.
---
## Files Included
- Tabora_ExploratoryDataAnalysisSpotify2023.ipynb: Jupyter notebook with the Python code.
- spotift-2023.csv: Excel data for given problems.
---
## Software and Library Used
- Python (version 3.x)
- Jupyter Notebook
- pandas (Python Data Analysis Library)
- matplotlib.pyplot
- seaborn.lineplot
---
## Author
- Carl Johnsen M. Tabora
