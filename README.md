# Midterm 2 – STA 309

This project is comprised of two main components: an analysis of global dairy production and consumption, and a sentiment and audio analysis of Taylor Swift songs. The entire project is implemented in R, utilizing libraries such as tidyverse, tidytext, sf, and patchwork.

## 🥛 Part 1: Dairy Production and Consumption Analysis

The milk production and consumption data is sourced from Our World in Data. The script executes the following tasks:

- Loads both CSV files from GitHub
- Cleans and standardizes column names
- Converts year formats for consistency
- Merges the data with ISO3 country codes for effective mapping
- Generates visualizations

### Dairy Dashboard Features:
- A world map displaying milk production data for 2022
- A world map illustrating milk consumption per capita for 2022
- A global trend chart showing milk production from 1961 to 2022
- A scatter plot comparing production against consumption on a log scale

These visualizations effectively highlight regional disparities and long-term trends within the dairy industry.

## 🎤 Part 2: Taylor Swift Lyrics and Sentiment Analysis

Lyrics and Spotify metadata are obtained from a publicly available dataset at [Taylor Swift Data](link). The script performs the following functions:

- Extracts the repository containing the dataset
- Automatically detects album folders that contain .txt lyric files
- Loads the lyrics for two selected albums
- Cleans the text by removing HTML remnants, “embed” artifacts, and punctuation

### Word Clouds:
Two word clouds are generated—one for each album—after filtering out stop words.

## 📊 Sentiment Analysis and Spotify Audio Features

The analysis uses both Bing and AFINN lexicons to calculate positive and negative sentiment counts as well as numeric sentiment scores. Song titles are normalized to facilitate the integration of sentiment data with Spotify audio features.

## Final Dashboard

The combined dashboard presents:

- A sentiment comparison chart
- Four scatter plots linking sentiment with:
  - Danceability
  - Energy
  - Valence
  - Tempo

All components are seamlessly integrated using patchwork.

## ✔️ Summary

This project showcases:

- Data wrangling and visualization techniques in R
- Mapping capabilities utilizing sf and naturalearth
- Text mining and sentiment analysis methods
- Integration of lyrical sentiment with Spotify audio metadata
- Creation of multi-panel dashboards using patchwork

For further details, feel free to explore the code and visualizations included in this repository.
