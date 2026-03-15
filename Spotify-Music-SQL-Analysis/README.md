# Spotify Music Analysis Using SQL

## Project Overview

This project explores a Spotify track dataset using SQL to analyse patterns in song popularity, artist representation, and audio characteristics. The analysis focuses on identifying trends in genres, song features such as danceability and energy, and the relationship between these attributes and track popularity.

The project was designed to simulate a real-world exploratory data analysis workflow used by data analysts in the music industry.

---

## Dataset

The dataset contains **114,000 Spotify tracks** with audio and metadata attributes including:

- Track name  
- Artist name  
- Genre  
- Popularity score  
- Danceability  
- Energy  
- Acousticness  
- Valence  
- Tempo  
- Duration  

Each genre contains approximately **1,000 tracks**, indicating that the dataset was intentionally balanced for analytical and machine learning purposes.

---

## Tools Used

- SQL  
- SQLite  
- DB Browser for SQLite  

---

## Data Preparation

Before conducting the analysis, several data checks were performed:

- Verified the total number of songs in the dataset  
- Checked for missing values in key columns such as track name, artist, and genre  
- Identified duplicate track and artist combinations  
- Examined the range of popularity scores  
- Calculated summary statistics for key audio features  
- Created a cleaned SQL view (`clean_spotify`) to filter out incomplete records  

---

## Analysis Questions

The SQL analysis explored several questions:

- Which artists appear most frequently in the dataset?
- Which tracks have the highest popularity scores?
- Which genres have the highest average popularity?
- Which genres have the highest danceability and energy levels?
- What are the longest songs in the dataset?
- Which songs combine high popularity and high danceability?
- Which songs have extremely high acousticness levels?

Additional ranking analysis was used to identify the **most popular songs within each genre**.

---

## Key Insights
## Key Insights

- The dataset contains an equal number of tracks for each genre (approximately 1000 tracks per genre), indicating that the dataset was intentionally balanced to allow fair comparisons across musical styles.

- The song **“I'm Good (Blue)” by David Guetta and Bebe Rexha** consistently appeared as the highest-ranked track in the popularity-based analysis, achieving a popularity score of **98** and also appearing in the results for highly energetic songs with an energy value of **0.965**.

- The track **“Freaks” by Surf Curse** also appeared repeatedly in the high-popularity and high-energy analysis results, with a popularity score of **86** and an energy level of **0.941**, indicating that energetic songs tend to perform well in terms of popularity.

- **“After LIKE” by IVE** appeared among the highly ranked songs in the dataset with a popularity score of **88** and strong audio feature values, highlighting how contemporary pop tracks often combine high popularity with strong rhythmic and energetic characteristics.

- Analysis of audio features suggests that songs with **higher energy and danceability values tend to appear more frequently among the most popular tracks**, indicating a potential relationship between energetic production styles and listener engagement.

- Ranking analysis by genre revealed that top-performing songs vary across genres, but high-energy electronic and pop tracks frequently appear among the most popular songs in the dataset.

---

## Example SQL Skills Demonstrated

This project demonstrates several core SQL skills including:

- `SELECT`
- `WHERE`
- `GROUP BY`
- `ORDER BY`
- `COUNT()`
- `AVG()`
- `MIN()` / `MAX()`
- window functions such as `RANK()`

These queries were used to perform exploratory analysis and compare patterns across different genres and song characteristics.

---

## Project Structure



