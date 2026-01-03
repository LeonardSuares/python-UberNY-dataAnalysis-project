# Uber New York Data Analysis

A comprehensive Streamlit dashboard for analyzing Uber pickup patterns in New York City (Jan-June 2015). This project utilizes Plotly for interactive data exploration and Streamlit's multi-page architecture for a clean user experience.

## Key Features
* **Temporal Demand Heatmaps:** Visualize peak hours and days across the first half of 2015.
* **Dispatching Base Intelligence:** Analyze trip volume vs. active vehicles to determine base efficiency.
* **Interactive Filtering:** Explore demand patterns across different months and weekdays.
* **Automated ETL:** Centralized data cleaning and feature engineering in `utils.py`.

## Tech Stack
* **Python** (Pandas, NumPy)
* **Streamlit** (Dashboarding & Session State)
* **Plotly** (Interactive Geospatial & Temporal Visualizations)

## 📂 Installation
1. Clone the repo.
2. Place CSV files in the `data/` folder.
3. Run `streamlit run Home.py`.
