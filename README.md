# Spotify Music Popularity Prediction

## Project Introduction

This project demonstrates how to interact with the **Spotify Web API**, collect music data programmatically, and analyze it for patterns and insights. By building a structured dataset of tracks, artists, and audio features, the project showcases how data science techniques can be applied to music analytics.

## Main Idea

The core idea is to:

* **Fetch data from Spotify’s API** (tracks, audio features, metadata).
* **Build a dataset** that can be reused for exploration and analysis.
* **Perform exploratory data analysis (EDA)** to uncover trends and relationships (such as audio features vs. popularity).
* Optionally, experiment with **basic predictive modeling** (e.g., predicting popularity or clustering tracks).

This pipeline bridges data engineering (API ingestion, dataset creation) and data analysis (visualization, EDA, modeling).

## Installation

1. **Clone the repository**

```bash
git clone https://github.com/kashyap-1234/spotify.git
cd spotify
```

2. **Create and activate a virtual environment**

```bash
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
```

3. **Install dependencies**

```bash
pip install spotipy pandas numpy matplotlib seaborn scikit-learn jupyter
```

4. **Set Spotify API credentials**
   Create a Spotify developer app at [https://developer.spotify.com/dashboard/](https://developer.spotify.com/dashboard/) and export your credentials:

```bash
export SPOTIPY_CLIENT_ID="<your_client_id>"
export SPOTIPY_CLIENT_SECRET="<your_client_secret>"
export SPOTIPY_REDIRECT_URI="http://localhost:8888/callback"
```

5. **Run the notebooks**

* `Spotify_API_Call.ipynb` → Fetch data from Spotify and create `dataset.csv`.
* `BDM_Project_Code.ipynb` → Perform analysis and visualization.

## Results

* A **curated dataset** (`dataset.csv`) containing track metadata and audio features.
* **Exploratory analysis** with visualizations highlighting distributions, correlations, and feature importance.
* Insights into how audio features (like energy, valence, danceability) relate to track popularity.
* A **final report** (`BDM_Final_Report.pdf`) summarizing findings, plots, and potential modeling directions.

The results demonstrate how easily accessible Spotify data can be transformed into meaningful insights through data wrangling and analysis.
