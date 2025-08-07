# Video Game Sales Forecasting

**Sprint 5 Project - TripleTen Data Science Bootcamp**

## 📋 Project Overview

This project demonstrates comprehensive **Video Game Market Analysis and Business Intelligence** using historical gaming data to identify patterns that determine game success. Working as an analyst for online game store Ice, the analysis focuses on market trends, platform lifecycles, regional preferences, and statistical validation to inform 2017 marketing campaign strategies and identify potential high-performing games.

## 🎯 Objectives

- Analyze video game market data to identify patterns determining game success
- Evaluate platform lifecycles and performance trends for strategic planning
- Conduct comprehensive regional market analysis across North America, Europe, and Japan
- Investigate genre preferences and their impact on sales performance
- Apply statistical hypothesis testing to validate market assumptions
- Generate actionable business intelligence for 2017 marketing campaign planning

## 🛠️ Technologies & Libraries Used

- **Python** - Primary programming language
- **Pandas** - Data manipulation, aggregation, and preprocessing
- **NumPy** - Numerical computations and data transformations
- **SciPy** - Statistical hypothesis testing (t-tests)
- **Matplotlib** - Data visualization and trend analysis
- **Seaborn** - Statistical plots and heatmap visualizations
- **Jupyter Notebook** - Interactive development environment

## 📊 Key Analyses Performed

### **Data Preprocessing & Quality Assessment**
1. **Data Cleaning & Standardization**
   - Standardized column names and converted data types for temporal analysis
   - Handled missing values: filled ESRB ratings with 'Unknown', removed incomplete entries
   - Converted 'TBD' user scores to numeric format for statistical analysis
   - Calculated total sales across all regions (NA, EU, JP, Other)

2. **Data Quality Analysis**
   - Identified substantial missing values in critic scores, user scores, and ratings
   - Analyzed missing value patterns related to release years and regional differences
   - Assessed data completeness for reliable statistical testing

### **Temporal & Platform Lifecycle Analysis**
3. **Game Release Trends (1980-2016)**
   - Peak release period: 2006-2011 with maximum in 2009-2010
   - Identified correlation between economic recession (2006-2008) and increased game releases
   - Selected relevant period (2007-2015) for 2017 prediction modeling

4. **Platform Performance & Lifecycle Analysis**
   - **Consistent Performers**: PS4, XOne, PC maintained steady sales
   - **Market Exits**: Gen, SCD, TG16 disappeared from market
   - **Declining Platforms**: DS, PS2, Wii, Xbox360 showed downward trends
   - **Platform Lifecycle**: Established typical 10-year platform lifespan

### **Market Analysis & Business Intelligence**
5. **Genre Performance Analysis**
   - **Market Leaders**: Action games dominated across all regions
   - **Secondary Genres**: Sports and Shooter games showed strong performance
   - **Genre Advantage**: Interactive and simulation-based games outperformed single-purpose titles
   - **Market Share Calculation**: Quantified genre distribution for strategic planning

6. **Review Score Impact Assessment**
   - Analyzed correlation between critic/user scores and sales performance
   - Platform-specific analysis (Wii) revealing score-sales relationships
   - Cross-platform game comparison for multi-release titles

### **Regional Market Analysis**
7. **Cross-Regional Platform Comparison**
   - **Market Size Ranking**: North America > Europe > Japan
   - Platform preference analysis across three major regions
   - Identified regional variations in platform adoption

8. **Regional Genre Preferences**
   - Action genre dominance confirmed across all regions
   - Regional variations in secondary genre preferences
   - Cultural market differences in game type preferences

9. **ESRB Rating Impact by Region**
   - E-rated and Unknown-rated games showed strong cross-regional performance
   - Notable finding: Japan sales increase with 'Unknown' ESRB ratings
   - Regional regulatory and cultural factors affecting rating impact

### **Statistical Hypothesis Testing**
10. **Platform User Rating Comparison**
    - **H₀**: Xbox One and PC platforms have equal average user ratings
    - **H₁**: Platform ratings differ significantly
    - **Result**: Failed to reject H₀ (p-value = 0.12 > α = 0.05)
    - **Finding**: Platform choice doesn't significantly impact user engagement

11. **Genre User Rating Comparison**
    - **H₀**: Action and Sports genres have equal average user ratings  
    - **H₁**: Genre ratings differ significantly
    - **Result**: Rejected H₀ (p-value = 0.002 < α = 0.05)
    - **Finding**: Genre significantly influences user engagement and satisfaction

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
