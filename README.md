# Streaming Platform Content Analysis

## Overview
This project analyzes and compares movie and TV show catalogs across four major streaming platforms: **Netflix**, **Hulu**, **Disney+**, and **Amazon Prime**. The notebook conducts data preprocessing, cleaning, and exploratory analysis to uncover patterns in content distribution across these platforms.

## Dataset
The analysis uses four separate datasets containing comprehensive listings of available content on each platform. Each dataset includes:
- **Basic Info**: Title, type (Movie/TV Show), release year
- **Content Details**: Cast, directors, ratings, duration
- **Metadata**: Country of origin, genres, date added to platform
- **Descriptions**: Plot summaries for each title

**Source**: [Netflix Shows Dataset on Kaggle](https://www.kaggle.com/datasets/shivamb/netflix-shows)

## Dataset Size
| Platform | Records | Total Fields |
|----------|---------|--------------|
| Amazon Prime | 9,668 | 11 |
| Hulu | 3,073 | 11 |
| Disney+ | 1,450 | 11 |
| Netflix | 8,807 | 11 |

## Key Features
- **Data Cleaning**: Standardizes missing values, handles data type conversions, and normalizes inconsistencies across datasets
- **Text Processing**: Lowercases descriptions for uniform analysis
- **Multi-Platform Integration**: Consolidates data with platform identifiers for comparative insights
- **Content Clustering**: Groups similar titles using similarity metrics for recommendation potential

## Technologies Used
- **Data Processing**: Pandas, NumPy
- **Visualization**: Plotly, Matplotlib, Seaborn
- **Text Analysis**: WordCloud, Regular Expressions
- **Environment**: Python, Jupyter Notebook

## Workflow
1. Load and inspect individual platform datasets
2. Standardize data types and formats across all datasets
3. Clean missing values and handle inconsistencies
4. Consolidate into unified multi-platform dataset
5. Perform exploratory analysis and clustering
6. Generate visualizations for insights

## Key Insights Potential
- Content distribution patterns across platforms
- Genre preferences and trends by streaming service
- Missing data patterns and data quality issues
- Similarity-based content recommendations
- Temporal trends in content additions

## Getting Started
Ensure you have the required CSV files in your working directory:
- `amazon_prime_titles.csv`
- `hulu_titles.csv`
- `disney_plus_titles.csv`
- `netflix_titles.csv`

Run the notebook cells sequentially to reproduce the analysis pipeline.

## Notes
- Some fields contain missing values represented as NaN or "No Data"
- The `date_added` field is converted to year format for simplified temporal analysis
- Hulu's cast data is stored as float64 (likely due to missing values)
