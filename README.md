# Spotify Top 200: Market Intelligence & Longevity Analysis

![Project Status](https://img.shields.io/badge/Status-Complete-green)
![Tools](https://img.shields.io/badge/Tools-Python%20%7C%20Power%20BI%20%7C%20Spotify%20API-blue)

## 📌 Project Overview
An end-to-end Business Intelligence solution that analyzes the lifecycle of songs on the Spotify Top 200 charts. The project identifies the mathematical impact of collaborations on chart longevity and visualizes global streaming trends through a sophisticated, multi-page Power BI dashboard.

## 🛠️ Technical Architecture

### 1. Data Acquisition & Enrichment
* **Web Scraping:** A Python-based pipeline using `BeautifulSoup`/`Selenium` to extract daily rankings and stream counts from regional Spotify charts.
* **Spotify API Integration:** Automated metadata retrieval to fetch high-resolution album art and artist genres, enriching the raw scraped data.
* **ETL Process:** Cleaned and standardized "dirty" web data using Regex and Python, handling regional naming variations and missing values.

### 2. Data Modeling (Snowflake Schema)
To reduce redundancy and optimize performance, I implemented a **Snowflake Schema**:
* **Fact Table:** Centralized transactional data (Ranks, Streams).
* **Dimension Tables:** Normalized tables for `Artists`, `Tracks`, `Geography`, and a custom `DateTable`.
* **Advanced Logic:** Utilized **Disconnected Tables** and **Slicer Syncing** to enable dynamic highlighting of monthly performance within a 12-month historical context.

### 3. Dashboard Design Philosophy
The report is divided into three "Color Zones" to provide immediate contextual cues:
* 🟢 **Artist Spotlight (Green):** Granular deep-dives into individual performer catalogs and geographic reach.
* 🟣 **Global Trends (Purple):** Macro-level market analysis, genre dominance treemaps, and success-correlation scatter plots.
* 🟡 **Chart History (Yellow):** Time-series analysis focusing on seasonality, chart churn rates, and collaboration vs. solo performance ROI.

## 📈 Key Insights
* **The Collaboration Multiplier:** Collaborative tracks demonstrate an 18% higher retention rate than solo tracks.
* **Chart Churn:** Identified a 20% churn rate in the Top 10, highlighting the "Legacy Lock" in high-performing positions.
* **Seasonal Peaks:** Identified October as a strategic "Release Vacuum" for maximizing peak chart positions before the Q4 holiday rush.


## 👤 Contact
Ahmed Fawzy- [https://www.linkedin.com/in/ahmedfawzy226497/]
