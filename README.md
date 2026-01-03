# Uber NY Operations Intelligence Dashboard

An interactive, multi-page data analytics platform built with **Streamlit** and **Plotly** to visualize 2015 Uber pickup trends in New York City. This project transforms raw CSV datasets into actionable insights regarding temporal demand and base efficiency.



---

## Key Features

* **Temporal Demand Heatmaps:** High-resolution visualization of "Hour vs. Day" demand patterns using Plotly's interactive scaling.
* **Base Performance Metrics:** Comparative analysis of dispatching bases utilizing FOIL data to calculate **Trips-per-Vehicle** efficiency.
* **Granular Location Lookup:** A deep-dive tool for individual **Location IDs**, allowing users to identify peak hours for specific NYC zones.
* **Persistent Navigation:** sidebar-controlled multi-page architecture for seamless exploration of different data facets.
* **Live Data Auditing:** Integrated expanders for raw data inspection, synced to user-defined filters.

---

## Tech Stack

* **Language:** `Python 3.x`
* **Core Libraries:** `Pandas`, `NumPy`
* **Interactive Visuals:** `Plotly Express`, `Plotly Graph Objects`
* **Framework:** `Streamlit` (Multi-page Architecture)
* **Memory Management:** Centralized ETL logic in `utils.py` using `@st.cache_data`.

---

## Project Architecture

```text
Uber-NY-Analysis/
├── Home.py               # Landing page & Executive KPIs
├── utils.py              # Centralized cleaning & feature engineering
├── data/
│   ├── uber-raw-data-janjune-15_sample.csv
│   └── Uber-Jan-Feb-FOIL.csv
└── pages/
    ├── 1_Temporal_Patterns.py  # Pairwise heatmaps & Weekday trends
    ├── 2_Base_Performance.py   # Dispatching base efficiency metrics
    └── 3_Location_Analysis.py  # Top zones & neighborhood lookup
