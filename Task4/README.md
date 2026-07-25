# Spotify Tracks EDA & Data Visualization

## Dataset Overview
The Spotify Tracks dataset contains musical features and popularity metrics across various genres.

## Visualizations & Key Insights

### 1. Popularity Distribution
![Popularity Distribution](images/chart1_popularity_dist.png)
* **Insight:** Popularity is right-skewed with a large cluster at score 0.

### 2. Audio Features Heatmap
![Correlation Heatmap](images/chart2_correlation_heatmap.png)
* **Insight:** Strong positive correlation between loudness and energy; negative correlation between energy and acousticness.

### 3. Energy vs. Loudness
![Energy vs Loudness](images/chart3_energy_vs_loudness.png)
* **Insight:** Track energy increases predictably with higher loudness levels.

### 4. Genre vs. Popularity
![Genre Boxplot](images/chart4_genre_popularity_boxplot.png)
* **Insight:** Mainstream genres show higher baseline popularity with fewer extreme outliers.

### 5. Danceability vs. Valence
![Danceability vs Valence](images/chart5_danceability_vs_valence.png)
* **Insight:** Tracks designed for dancing strongly align with happier acoustic moods.

### 6. Song Duration Distribution
![Duration Violinplot](images/chart6_duration_violin.png)
* **Insight:** Streaming tracks strongly prefer a 3–4 minute duration window.

## Overall Conclusions
- Energy and loudness dominate modern track production standards.
- Commercial viability strongly favors track lengths between 3 and 4 minutes.
- Danceability and positivity (valence) exhibit high co-occurrence.
