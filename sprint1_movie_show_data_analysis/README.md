# Movie & TV Show Data Analysis

**Sprint 1 Project - TripleTen Data Science Bootcamp**

## 📋 Project Overview

This project focuses on **Data Preprocessing & Exploratory Data Analysis** of movie and TV show datasets. The goal was to understand viewing patterns, content trends, and analyze the entertainment industry landscape through comprehensive data analysis.

## 🎯 Objectives

- Perform thorough data cleaning and preprocessing on entertainment datasets
- Conduct exploratory data analysis to identify viewing patterns and trends
- Create meaningful visualizations to communicate insights about content ratings, genres, and release patterns
- Apply statistical analysis techniques to understand the entertainment industry

## 🛠️ Technologies & Libraries Used

- **Python** - Primary programming language
- **Pandas** - Data manipulation and cleaning
- **NumPy** - Numerical computations
- **Matplotlib** - Data visualization
- **Seaborn** - Statistical data visualization
- **Jupyter Notebook** - Interactive development environment

## 📊 Key Analyses Performed

1. **Data Quality Assessment**
   - Identified and handled missing values
   - Detected and addressed outliers
   - Standardized data formats and types

2. **Content Analysis**
   - Distribution of content by genre
   - Release year trends and patterns
   - Rating distributions across different content types

3. **Trend Analysis**
   - Popular genres over time
   - Content production patterns
   - Regional content preferences

## 📈 Key Findings

- **Data Cleaning Challenges**: Identified and corrected column naming issues including inconsistent spacing, special characters (r0le → role), and case inconsistencies (TITLE → title)
- **Data Quality Issues**: Found encoding problems with special characters in actor names (e.g., "In??s Prieto" corrected to "Ines Prieto") requiring manual data correction
- **IMDb Score Distribution**: Developed rating categorization system with thresholds: Excellent (≥9.0), Good (7.0-8.9), Average (5.0-6.9), and Low (<5.0) for content evaluation
- **Dataset Structure**: Successfully processed movie and TV show data containing actor information, character roles, titles, release years, genres, IMDb scores, and vote counts
- **Data Manipulation Skills**: Created functions for filtering top-rated movies by decade, extracting cast lists for specific titles, and categorizing content by score ranges
- **Functional Programming**: Implemented reusable functions including `get_unique_top_movies()`, `get_top_movies_from_decade()`, `get_actors_for_title()`, and `categorize_imdb_score()` for data analysis
- **Data Processing Methodology**: Applied systematic approach to data cleaning including column renaming, data type validation, and content correction for analysis readiness

## 📁 Files in This Project

- `movie_shows_data_analysis.ipynb` - Main analysis notebook
- `README.md` - Project documentation

## � Navigation

← [Back to Main Portfolio](../README.md)

---

**Part of the TripleTen Data Science Bootcamp Portfolio** 