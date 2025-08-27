🎵 Spotify Songs Data Analysis
📌 Project Overview

This project analyzes a dataset of Spotify tracks to explore trends in song features such as:

Popularity

Danceability

Energy

Tempo

Genre

The goal is to clean the dataset, visualize patterns, and draw insights into music characteristics — such as top genres or how features have evolved over time.

📂 Dataset

We use the Spotify Tracks Dataset available on Kaggle/GitHub, which contains:

Metadata: track name, artist, album, release date, genre

Audio Features: popularity, danceability, energy, tempo, valence, instrumentalness, etc.

👉 Example source: Spotify Tracks Dataset on Kaggle

⚙️ Tools Used

Python → pandas, matplotlib

Excel (alternative for pivot tables and charts)

Jupyter Notebook / IDE for running the analysis

📊 Analysis Performed

Data Cleaning

Removed missing values and duplicates

Converted release_date to datetime

Exploratory Analysis & Visuals

Popularity Distribution → histogram

Danceability vs Popularity → scatter plot

Average Energy by Genre → bar chart

Tempo Trend Over Years → line chart

Top Genres by Popularity → bar chart

Insights

Certain genres (e.g., EDM, Hip-hop) show higher energy and popularity.

Danceable songs tend to have slightly higher popularity.

Tempo trends reveal how average song speed changes over time.

Some genres remain consistently popular across years.

🚀 How to Run
Using Python

Download the dataset (spotify_tracks.csv).

Install required libraries:

pip install pandas matplotlib


Run the Jupyter Notebook or Python script:

import pandas as pd
import matplotlib.pyplot as plt

df = pd.read_csv('spotify_tracks.csv')
df = df.dropna(subset=['popularity','danceability','energy','tempo','track_genre'])
df['popularity'].hist(bins=30)
plt.show()


📈 Business / Research Value

Helps understand listener preferences (danceability, energy, tempo).

Identifies top genres and evolving music trends.

Useful for music recommendation systems and market research.