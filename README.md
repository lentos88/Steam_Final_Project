# Steam Games Data Analysis Project

## Overview

This project analyzes Steam games data to uncover insights about game quality, popularity, consistency, and monetization. Using Python-based data analysis and exploratory data analysis (EDA), the project focuses on building meaningful KPIs that help evaluate sustainable game success, identify top-performing titles, and surface hidden gems across genres.

The analysis combines multiple datasets, performs extensive data cleaning and preparation, and applies custom indices to support data-driven storytelling.

---

## Project Objectives

* Clean, standardize, and merge multiple Steam-related datasets
* Explore relationships between ratings, reviews, genres, and release years
* Define and calculate business-oriented KPIs for game performance
* Identify top games, consistent performers, and under-the-radar high-quality games
* Support insights with clear visualizations and structured analysis

---

## Data Sources

The project is based on multiple Steam datasets, including:

* Game metadata (name, release year, genres)
* Ratings and reviews (English reviews count, average rating)
* Popularity and ranking-related fields

> Note: Dataset merging required careful standardization of key columns (game names) prior to analysis.

---

## Data Cleaning & Preparation

The data preparation process was divided into **pre-EDA** and **post-merge** stages:

### Pre-Merge Cleaning

* Standardized key columns (game names)
* Removed leading/trailing whitespaces
* Renamed columns for consistency

### Post-Merge Cleaning

* Handled missing values, especially in the `genres` column
* Filtered irrelevant or non-core genres
* Addressed negative anomalies and invalid values
* Converted data types to ensure analytical accuracy

### Genre Processing

* Split multi-genre fields
* Exploded genre rows to allow genre-level analysis
* Filtered to a defined set of core genres

---

## Exploratory Data Analysis (EDA)

The EDA phase focused on understanding:

* Distribution of rating scores
* Distribution of number of reviews
* Relationship between ratings and popularity
* Differences across genres and release years

Key visual analyses include:

* Rating score distributions
* Review count distributions
* Rating vs. reviews correlation
* Top games by number of reviews

---

## Key Performance Indicators (KPIs)

### KPI 1 – Sustainable Game Success Index (SGSI)

A composite metric designed to evaluate long-term game success by combining:

* Rating quality
* Popularity signals
* Consistency over time

#### Supporting Metrics:

* **Top Games Performance Index (TGPI)** – highlights the strongest performers
* **Consistency Score** – rewards stable, long-term engagement
* **Player Experience & Engagement indicators**
* **Player Satisfaction vs. Monetization** – explores trade-offs between reviews and revenue proxies

---

### KPI 2 – Games Released per Year

Analyzes release trends over time to:

* Identify growth or saturation periods
* Understand market dynamics
* Contextualize performance by release year

---

### KPI 3 – Composite Score (Quality + Popularity)

Combines:

* Average rating
* Number of reviews

This KPI balances quality perception with audience reach.

---

### KPI 4 – Hidden Gems Score

Designed to surface games that:

* Have high ratings
* Maintain relatively low review counts

These games represent strong quality with untapped popularity potential.

---

## Tools & Technologies

* **Python**

  * Pandas
  * NumPy
  * Matplotlib / Seaborn
* **Jupyter Notebook**
* Data visualization and statistical exploration

---

## Project Structure

├── steam_final_project.ipynb - Main analysis notebook
├── README.md - Project documentation
├── games_description.csv
├── games_ranking.csv
├── steam_df.csv
├── Dashboard - Tableau dashboard

---

## Key Insights

* High ratings do not always correlate with high popularity
* Certain genres consistently outperform others in player satisfaction
* "Hidden gems" exist across multiple genres and release years
* Balancing quality and reach is critical for sustainable success

---

## How to Run the Project

1. Open `steam_final_project.ipynb`
2. Run all cells from top to bottom
3. Review visualizations and KPI outputs

---

## Authors

Ofir Ben-Harush, Tal Ezra, Neta Shtayer, Zvi Fuchs, Yelena Zamansky Glazer, Tehila Hamdi\
Python | SQL | Tableau

---

## Notes

This project was created as part of a Data Analyst course final project and demonstrates end-to-end data analysis, KPI design, and data storytelling skills.
