# Airbnb Market Performance and Listing Insights Dashboard

## Project Overview

This project explores Airbnb listing performance, pricing patterns, host performance, and review activity across 10 cities.

The goal was to prepare and analyse Airbnb listing and review data, identify useful market insights, and present the findings through an interactive Power BI dashboard.

## Project Objectives

- Clean and prepare the original Airbnb datasets.
- Analyse listing characteristics and pricing patterns.
- Examine host performance indicators.
- Explore review activity and listing scores.
- Build an interactive dashboard to communicate findings.

## Tools and Technologies

- **Python:** Data cleaning, preparation and analysis.
- **Jupyter Notebook:** Python analysis and SQL queries.
- **SQLite3:** Database creation, storage and querying.
- **Power BI:** Dashboard development and visualisation.

## Data Preparation

The project began with two original CSV datasets:

- Listings dataset
- Reviews dataset

The datasets were cleaned and transformed to prepare them for analysis and visualisation.

Three additional CSV files were created during the preparation process:

- `listings_clean.csv`
- `reviews_per_month.csv`
- `reviews_per_listing.csv`

An SQLite database, `airbnb.db`, was also created to store and query the project data.

Two data dictionaries were also created to explain the datasets and their columns. They are supporting documentation and are not currently included in this repository.

## Analysis and Dashboard

The project includes four Power BI dashboard pages:

1. **Airbnb Market Overview:** An overview of Airbnb listings across the selected cities.
2. **Pricing and Property Analysis:** Exploration of listing prices and property characteristics.
3. **Host Performance Analysis:** Examination of host-related performance indicators.
4. **Review Activity and Listing Scores:** Analysis of review patterns and listing-level scores.

Python was used for data preparation and analysis, while SQLite3 was used for SQL queries. Power BI was used to develop the interactive dashboard.

## Dashboard Screenshots

### 1. Airbnb Market Overview
![Airbnb Market Overview]()

### 2. Pricing and Property Analysis
![Pricing and Property Analysis](screenshots/filename.png)

### 3. Host Performance Analysis
![Host Performance Analysis](screenshots/filename.png)

### 4. Review Activity and Listing Scores
![Review Activity and Listing Scores](screenshots/filename.png)
## Data Quality Checks

Some of the data quality checks carried out included:

- Checking for missing values.
- Identifying duplicate records.
- Checking relationships between listings and reviews.
- Identifying listings with zero prices or zero accommodation capacity.
- Examining missing listing-level review information.

The reviews dataset contained repeated `review_id` values, but the combination of `listing_id` and `review_id` was unique. No orphan review records were identified.

## Key Findings

- The dataset contained 279,712 listings across 10 cities.
- The reviews dataset contained over 5.3 million records.
- Paris had the highest number of listings, with 64,690.
- 86,156 listings had no associated review records.
- Review activity varied over time, with activity reaching its highest levels around 2019.

## Limitations

- Listing prices were recorded in local currencies, so direct price comparisons across cities require caution.
- The reviews dataset contained review IDs and dates but not the actual review text or individual review ratings.
- Some listing attributes contained missing values.
- The dataset did not include occupancy, booking or realised revenue information.
- The final period of review activity may be incomplete.

## Project Files

The repository contains the project notebook, datasets and supporting analysis files, including:

- Original and processed CSV datasets.
- SQLite database (`airbnb.db`).
- Jupyter Notebook containing Python analysis and SQL queries.
- Power BI dashboard file (`.pbix`).
- Dashboard screenshots.
- Data Quality Assessment.
- KPI Definition Sheet.
- Executive Summary.
- Validation evidence.

## Conclusion

This project demonstrates a practical data analytics workflow, from data cleaning and preparation to database querying, exploratory analysis and dashboard development.

The Power BI dashboard provides an interactive way to explore Airbnb market performance, listing characteristics, host indicators and review activity across the selected cities.
