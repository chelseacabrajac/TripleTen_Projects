# Movie & TV Show Data Analysis

**Sprint 1 Project - TripleTen Data Science Bootcamp**

## 📋 Project Overview

This project demonstrates **Data Analysis with Pandas** through systematic data cleaning, manipulation, and function creation using a comprehensive movie and TV show dataset. The focus was on developing practical pandas skills including DataFrame operations, data filtering, indexing, and creating reusable functions for data analysis tasks.

## 🎯 Objectives

- Master fundamental pandas operations for data cleaning and manipulation
- Practice DataFrame indexing, filtering, and data correction techniques  
- Develop reusable functions for common data analysis tasks
- Learn systematic approaches to data quality assessment and correction
- Apply conditional logic and data categorization methods

## 🛠️ Technologies & Libraries Used

- **Python** - Primary programming language
- **Pandas** - Data manipulation, cleaning, and analysis
- **Jupyter Notebook** - Interactive development environment

## 📊 Key Analyses Performed

1. **Data Cleaning & Column Standardization** (Task 1)
   - Corrected column naming issues (spaces, special characters, case inconsistencies)
   - Standardized column names: `r0le` → `role`, `TITLE` → `title`, `imdb sc0re` → `imdb_score`
   - Removed unnecessary whitespace from column headers

2. **Data Quality Correction** (Task 2)
   - Identified and corrected encoding issues with special characters
   - Fixed misspelled actor name: "In??s Prieto" → "Ines Prieto"
   - Used `.loc[]` indexing for precise data correction

3. **Data Filtering & Actor Analysis** (Task 3)
   - Implemented conditional filtering to find all works by specific actors
   - Extracted relevant columns (title, release_year, imdb_score, genres)
   - Created actor-specific filmography profiles

4. **High-Rating Content Identification** (Task 4)
   - Filtered movies with IMDb scores ≥ 9.0
   - Applied set operations to remove duplicate titles
   - Created curated lists of top-rated content

5. **Function Development** (Tasks 5-8)
   - **`get_unique_top_movies(min_score)`**: Finds unique high-rated movies above score threshold
   - **`get_top_movies_from_decade(decade_start, min_score)`**: Retrieves top movies from specific decades
   - **`get_actors_for_title(title)`**: Lists all actors in a given movie/show as formatted string
   - **`categorize_imdb_score(title)`**: Categorizes content by rating (Excellent/Good/Average/Low)

## 📈 Key Findings & Technical Skills Demonstrated

- **Data Cleaning Mastery**: Successfully corrected systematic column naming issues including inconsistent spacing, special characters (`r0le` → `role`), and case inconsistencies (`TITLE` → `title`)

- **Precision Data Correction**: Resolved encoding problems with special characters in actor names (e.g., "In??s Prieto" → "Ines Prieto") using targeted `.loc[]` indexing

- **Rating Categorization System**: Developed comprehensive IMDb score classification with thresholds: Excellent (≥9.0), Good (7.0-8.9), Average (5.0-6.9), and Low (<5.0)

- **Dataset Structure Mastery**: Successfully processed complex entertainment data containing actor information, character roles, titles, release years, genres, IMDb scores, and vote counts across movies and TV shows

- **Advanced Filtering Techniques**: Implemented multi-condition filtering for decade-based analysis, actor-specific searches, and score-based content curation

- **Functional Programming Implementation**: Created four reusable, parameterized functions:
  - `get_unique_top_movies()` - Threshold-based movie filtering
  - `get_top_movies_from_decade()` - Time-period and score filtering
  - `get_actors_for_title()` - Cast extraction and formatting
  - `categorize_imdb_score()` - Automated content rating classification

- **Data Processing Methodology**: Applied systematic approach combining DataFrame operations, set operations for duplicate removal, string manipulation for output formatting, and conditional logic for categorization

## 📁 Files in This Project

- `movie_shows_data_analysis.ipynb` - Main analysis notebook
- `README.md` - Project documentation

## 🔗 Navigation

← [Back to Main Portfolio](../README.md)

---

**Part of the TripleTen Data Science Bootcamp Portfolio** 