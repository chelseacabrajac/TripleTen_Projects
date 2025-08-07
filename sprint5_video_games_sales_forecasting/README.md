# Video Game Sales Forecasting

**Sprint 5 Project - TripleTen Data Science Bootcamp**

## 📋 Project Overview

This project focuses on **Predictive Modeling & Machine Learning** to forecast video game sales performance. The analysis applies advanced machine learning techniques to predict sales and identify key factors that influence game success across different markets.

## 🎯 Objectives

- Build robust predictive models to forecast video game sales performance
- Apply machine learning techniques for accurate sales prediction
- Analyze factors influencing game success in different regional markets
- Develop actionable insights for game development and marketing strategies

## 🛠️ Technologies & Libraries Used

- **Python** - Primary programming language
- **Pandas** - Data manipulation and feature engineering
- **NumPy** - Numerical computations
- **Matplotlib** - Data visualization
- **Seaborn** - Statistical data visualization
- **Jupyter Notebook** - Interactive development environment

## 📊 Key Analyses Performed

1. **Feature Engineering**
   - Game attribute analysis (genre, platform, rating)
   - Regional market segmentation
   - Temporal trend analysis

2. **Predictive Modeling**
   - Linear regression for baseline predictions
   - Random Forest for non-linear relationships
   - Gradient boosting for ensemble predictions
   - Model comparison and validation

3. **Market Analysis**
   - Regional sales pattern identification
   - Platform performance across markets
   - Genre popularity trends over time

## 📈 Key Findings

- **Platform Lifecycle Analysis**: Identified platforms that disappeared from market (Gen, SCD, TG16g) vs. those with consistent sales (PS4, XOne, PC), while platforms like DS, PS2, Wii, Xbox360 showed declining trends from early 2000s peak to 2016
- **Genre Market Dominance**: Action games dominated across all regions in both preference and sales, followed by Sports and Shooter games, due to their interactive and real-life simulation capabilities versus one-dimensional gaming experiences
- **Regional Market Distribution**: North America leads in total sales, followed by Europe, then Japan, with notable finding that Japan sales significantly increased when ESRB rating was "Unknown"
- **Statistical Hypothesis Testing Results**: 
  - Xbox One vs PC user ratings: Failed to reject null hypothesis (p-value = 0.12), indicating no significant difference in user ratings between platforms
  - Action vs Sports genre ratings: Rejected null hypothesis (p-value = 0.002), confirming significant difference in user ratings between genres
- **Platform vs Genre Impact**: Statistical tests revealed that genre influences user engagement more significantly than platform choice, making genre the critical factor for marketing strategy
- **Data Quality Challenges**: Substantial missing values identified in user rating datasets, with cleaned data showing 0.35 mean difference between Xbox One and PC ratings, and 0.39 mean difference between Action and Sports genres
- **Business Intelligence**: Top marketing focus should be on Action, Sports, and Shooter games on PS4, XOne, and PC platforms, with E-rated and Unknown-rated games showing promising revenue across all regions
- **Strategic Recommendations**: North America and Europe identified as primary target markets for 2017 marketing campaigns, with genre selection being more critical than platform choice for market success

## 📁 Files in This Project

- `video_game_sales_forecasting.ipynb` - Main analysis notebook
- `README.md` - Project documentation

## 🔗 Navigation

← [Back to Main Portfolio](../README.md)

---

**Part of the TripleTen Data Science Bootcamp Portfolio**
