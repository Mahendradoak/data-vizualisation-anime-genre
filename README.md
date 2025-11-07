# Anime Genre Data Visualization and Analysis

A comprehensive dataset and analysis of anime titles, exploring genre trends, ratings, and characteristics over time. This repository contains processed data ready for visualization and statistical analysis.

## Dataset Overview

This repository contains anime data from **15,525 titles**, including detailed information about:
- Anime titles (English, Japanese, and synonyms)
- Genres and categories
- Ratings and scores
- Episode counts and duration
- Studios and producers
- Air dates and premiere information
- Synopsis and background information

## Files Description

### Raw Data
- **`raw_anime.csv`** (16.7 MB)
  - Complete anime dataset with 27 columns
  - Contains comprehensive information for each anime title
  - Includes metadata like animeID, names, genres, scores, episodes, studios, and more

### Processed Analysis Files

1. **`genre_trends_over_time.csv`**
   - Tracks genre popularity percentage and count by year
   - Shows how different genres have evolved over decades

2. **`average_genre_ratings_by_decade.csv`**
   - Average scores for each genre grouped by decade
   - Includes count of titles per genre/decade combination

3. **`average_genre_ratings_over_time.csv`**
   - Year-by-year average ratings for each genre
   - Detailed temporal analysis of genre quality trends

4. **`score_by_anime_type.csv`**
   - Compares average scores across anime types (TV, Movie, OVA, Special, ONA)
   - Includes count, standard deviation, and error metrics

5. **`score_by_episode_duration.csv`**
   - Analyzes relationship between episode duration and ratings

6. **`runtime_vs_score_by_type.csv`** (330 KB)
   - Detailed analysis of runtime impact on scores
   - Segmented by anime type

7. **`score_distribution_by_episode_count.csv`** (284 KB)
   - Distribution of scores based on total episode count
   - Helps identify patterns in series length vs. quality

### Additional Data
- **`cleaned_co2_population_poverty.csv`**
  - Environmental and demographic dataset (appears to be from a separate analysis)

## Key Insights from the Data

### Score by Anime Type
Based on the processed data:
- **TV Series**: Average score of 6.76 (4,111 titles)
- **Specials**: Average score of 6.48 (583 titles)
- **OVA**: Average score of 6.45 (1,673 titles)
- **ONA**: Average score of 5.99 (706 titles)
- **Movies**: Average score of 5.82 (32 titles analyzed)

### Genre Evolution
The dataset tracks genres from the 1970s to present, including:
- Action, Adventure, Comedy, Drama, Romance
- Sci-Fi, Fantasy, Mystery, Thriller
- Slice of Life, Shounen, Shoujo
- And many more...

## Data Source

The data appears to be sourced from MyAnimeList (MAL), as evidenced by:
- MAL IDs in the raw data
- Score metrics from MAL's rating system
- References to MAL URLs in related content

## Potential Use Cases

This dataset is ideal for:
- **Data Visualization Projects**: Create interactive dashboards showing anime trends
- **Statistical Analysis**: Explore correlations between genres, ratings, and time periods
- **Machine Learning**: Build recommendation systems or predictive models
- **Trend Analysis**: Study how anime genres and preferences have evolved
- **Academic Research**: Analyze cultural trends in Japanese animation

## Data Structure

### Main Raw Data Columns
- `animeID`: Unique identifier
- `name`, `title_english`, `title_japanese`: Various title formats
- `type`: TV, Movie, OVA, Special, ONA
- `genre`: List of genres for each title
- `studio`: Production studio
- `episodes`: Number of episodes
- `duration`: Episode duration
- `score`: Average rating (0-10 scale)
- `scored_by`: Number of users who rated
- `aired`: Air date information
- `synopsis`: Plot description
- And more...

## Getting Started

### Basic Usage

1. **Load the raw data**:
```python
import pandas as pd
anime_data = pd.read_csv('raw_anime.csv')
```

2. **Explore genre trends**:
```python
genre_trends = pd.read_csv('genre_trends_over_time.csv')
```

3. **Analyze ratings by type**:
```python
scores_by_type = pd.read_csv('score_by_anime_type.csv')
```

### Visualization Examples

The processed files are ready for visualization with tools like:
- **Matplotlib/Seaborn**: Create static plots and charts
- **Plotly**: Build interactive visualizations
- **Tableau/Power BI**: Import for business intelligence dashboards
- **D3.js**: Web-based interactive visualizations

## Data Quality Notes

- The dataset includes anime from 1970s to present
- Some entries may have missing or null values
- Genre information is stored as string representations of lists
- Dates are stored in structured JSON format in the raw data

## Contributing

If you use this dataset for analysis or visualization projects, consider:
- Sharing your findings and visualizations
- Reporting data quality issues
- Contributing additional processed datasets

## License

Please ensure compliance with MyAnimeList's terms of service when using this data. This dataset is intended for educational and research purposes.

## Acknowledgments

Data sourced from MyAnimeList (MAL), the world's largest anime and manga community and database.

---

**Repository**: data-vizualisation-anime-genre
**Last Updated**: 2025
**Total Anime Titles**: 15,525
