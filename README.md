# Exploratory Data Analysis of Spotify Song Data

This project performs an in-depth Exploratory Data Analysis (EDA) on a dataset of songs from Spotify. The analysis aims to uncover trends, patterns, and relationships within the audio features of songs, and to understand how these musical attributes have evolved over the years.

## 📌 Project Overview

The goal of this notebook is to explore a Spotify dataset containing nearly 170,000 songs spanning from the 1920s to the present day. By dissecting various audio features—such as `danceability`, `energy`, `valence`, and `acousticness`—the analysis seeks to answer questions like: How has music changed over the decades? What are the characteristics of the most popular songs? And what correlations exist between different audio features?

## 💾 Dataset

The project utilizes two main datasets:
1.  **`data.csv`**: Contains audio features for a vast collection of songs. Key columns include:
    - `acousticness`, `danceability`, `energy`, `instrumentalness`, `liveness`, `loudness`, `speechiness`, `tempo`, `valence`
    - `duration_ms`, `explicit`, `key`, `mode`, `year`, `artists`, `name`

2.  **`data_by_year.csv`**: An aggregated version of the main dataset, providing the average value of each audio feature for each year.

## ⚙️ Analysis Workflow

The project follows a systematic approach to explore the data from multiple angles.

### 1. Data Loading and Cleaning
- The datasets are loaded into pandas DataFrames.
- A preliminary check for missing values and duplicates is performed to ensure data quality.

### 2. Exploratory Data Analysis (EDA)
The core of the project involves a detailed examination and visualization of the song data:

- **Correlation Analysis**: A heatmap is generated to visualize the correlations between different audio features. This helps identify strong positive or negative relationships (e.g., between `energy` and `loudness`).
- **Feature Distribution**: The distribution of key audio features like `danceability`, `valence`, and `tempo` is analyzed to understand their typical ranges.
- **Top Artists Analysis**: The artists with the most songs in the dataset are identified.
- **Analysis of Top 10 Songs**: The notebook identifies and analyzes the audio features of the top 10 most popular songs in the dataset to see what characteristics they share.
- **Time Series Analysis**: The evolution of audio features over the decades is a central theme. Line charts are used to plot the average `danceability`, `acousticness`, `energy`, `valence`, etc., from the 1920s to the 2020s, revealing long-term trends in music production and taste.

## 📈 Analysis Conclusion

This exploratory analysis reveals fascinating trends in the evolution of music over the last century.

A key finding is the strong positive correlation between **energy and loudness**, confirming that higher-energy tracks are almost always louder. Conversely, **acousticness shows a strong negative correlation with energy**, indicating that acoustic-heavy music tends to be calmer.

The time-series analysis provides a clear narrative of musical change. Modern music is characterized by a significant increase in **danceability, energy, and loudness** compared to tracks from the early-to-mid 20th century. In contrast, **acousticness and instrumentalness have seen a steady decline**, reflecting the shift from acoustic instruments to electronic and synthesized production. Interestingly, **valence** (the musical positiveness) has also decreased over time, suggesting a trend towards more somber or melancholic moods in popular music.

Overall, the EDA successfully quantifies the stylistic shifts in music over the decades, providing a data-driven look into our collective musical history.

Dataset Name: Top Spotify Songs in 73 Countries (Daily Updated)     
Source: Kaggle Dataset     
LinkFile: [universal_top_spotify_songs](https://www.kaggle.com/datasets/asaniczka/top-spotify-songs-in-73-countries-daily-updated)

note     
Some plot codes cannot be viewed directly from the .ipynb file. To view the complete code, you can access it in the interactive-plot folder.
