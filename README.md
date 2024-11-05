# :musical_note: Exploratory Data Analysis on Spotify 2023 Dataset
#### Jump into the world of music data! This repository delves into an exploratory data analysis (EDA) of the [Most Streamed Spotify Songs 2023](https://www.kaggle.com/datasets/nelgiriyewithana/top-spotify-songs-2023) dataset, aiming to uncover hidden gems and shed light on popular music trends.<br />

## :ballot_box: Library Used
This project utilizes these powerful Python libraries:
- Numpy: is a library for scientific computing in Python. It provides efficient array operations, linear algebra functions, random number generation, and much more.
- Pandas: is a library built on NumPy and provides easy-to-use data structures and data analysis tools for the Python programming language.
- Matplotlib: is a Python 2D plotting library which produces publication-quality figures in a variety of hardcopy formats and interactive environments across platforms.
- Seaborn: is a Python data visualization library based on Matplotlib. It provides a high-level interface for creating attractive and informative statistical graphics.

## :interrobang: Guided Questions
- Overview of Dataset
  - How many rows and columns does the dataset contain?
  - What are the data types of each column? Are there any missing values?
  
- Basic Descriptive Statistics
  - What are the mean, median, and standard deviation of the streams column?
  - What is the distribution of released_year and artist_count? Are there any noticeable trends or outliers?

- Top Performers
  - Which track has the highest number of streams? Display the top 5 most streamed tracks.
  - Who are the top 5 most frequent artists based on the number of tracks in the dataset?

- Temporal Trends
  - Analyze the trends in the number of tracks released over time. Plot the number of tracks released per year.
  - Does the number of tracks released per month follow any noticeable patterns? Which month sees the most releases?

- Genre and Music Characteristics
  - Examine the correlation between streams and musical attributes like bpm, danceability_%, and energy_%. Which attributes seem to influence streams the most?
  - Is there a correlation between danceability_% and energy_%? How about valence_% and acousticness_%?

- Platform Popularity
  - How do the numbers of tracks in spotify_playlists, spotify_charts, and apple_playlists compare? Which platform seems to favor the most popular tracks?

- Advanced Analysis
  - Based on the streams data, can you identify any patterns among tracks with the same key or mode (Major vs. Minor)?
  - Do certain genres or artists consistently appear in more playlists or charts? Perform an analysis to compare the most frequently appearing artists in playlists or charts.

## :star2: Insights
Here are the specific insights I gained from the EDA:
- Popularity Trends
  - The dataset contains 953 rows and 24 columns, with a mix of object and integer.
  - The mean stream count is 514,137,424, with a median of 290,530,915 and a standard deviation of 566,856,949.
  - There is a growing trend of artist collaborations over the years, with a peak in recent decades. This suggests a shift towards more collaborative music projects.
  - The top 5 most streamed tracks are "Blinding Lights", "Shape of You", "Someone You Loved", "Dance Monkey", and "Sunflower - Spider-Man: Into the Spider-Verse".
  - The top 5 most frequent artists are Taylor Swift, The Weeknd, Bad Bunny, SZA, and Harry Styles.

- Feature Correlations
  - Danceability and energy are positively correlated with stream counts, indicating that more danceable and energetic songs tend to be more popular.
  - Tempo (bpm) is negatively correlated with danceability, suggesting faster songs are less danceable.
  - There is a moderate positive correlation between danceability and energy, and a weak positive correlation between acousticness and valence.

- Genre Analysis
  - The number of annual music releases has significantly increased in recent years, particularly since 2020, likely due to the expansion of the music industry and the rise of digital streaming platforms.
  - There is a seasonal pattern in music releases, with January and May seeing the highest number of releases, possibly timed with increased listener engagement during summer.

- Temporal Analysis
  - The number of tracks released per year has seen a significant increase, especially since 2020, reflecting the growth and expansion of the music industry.
  - The seasonal pattern in music releases, with peaks in January and May, suggests that artists and labels strategically plan their releases to capitalize on listener behavior and engagement.

- Platform-Specific Analysis
  - Spotify playlists contain the most tracks, indicating a focus on popular music, while Apple Music playlists have the fewest tracks, suggesting a more curated selection.

## :dart:  Challenges and Limitations
I encountered several challenges and limitations:
- The dataset required specific encoding (latin-1) to be correctly interpreted due to non-standard characters.
- The 'in_shazam_charts' column contained missing values, which were identified and handled using the .isnull() method.
- Missing values in the key column were filled with the string "NAN".
- Converting 'streams' column into numeric in order to get statistics.
- The quality of the plot, by adjusting the figure size using Matplotlib's figsize parameter, it can impact the reliability of the analysis.

## :card_file_box: File Structure
- README.md: This file (you're reading it!)
- spotify-2023.csv: File containing the downloaded dataset
- ECE2112-Exploratory-Data-Analysis.ipynb: Jupyter Notebook for Spotify 2023 Exploratory Data Analysis

## :information_source: Contact Information
Name: Prince Emmanuel Estoque<br /> 
Email: princeemmanuel.estoque.eng@ust.edu.ph
