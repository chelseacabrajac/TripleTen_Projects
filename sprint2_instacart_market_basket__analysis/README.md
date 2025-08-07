# Instacart Market Basket Analysis

**Sprint 2 Project - TripleTen Data Science Bootcamp**

## 📋 Project Overview

This project focuses on **Statistical Analysis & Data Insights** using Instacart grocery shopping data. The analysis aims to understand customer purchasing behavior, identify shopping patterns, and extract actionable insights about consumer preferences and product relationships.

## 🎯 Objectives

- Analyze customer purchasing behavior using real Instacart grocery data
- Perform comprehensive statistical analysis to understand shopping patterns
- Identify key insights about customer preferences and product relationships
- Apply statistical methods to derive business intelligence from transactional data

## 🛠️ Technologies & Libraries Used

- **Python** - Primary programming language
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computations and statistical operations
- **Matplotlib** - Data visualization
- **Seaborn** - Statistical data visualization
- **SciPy** - Statistical analysis and hypothesis testing
- **Jupyter Notebook** - Interactive development environment

## 📊 Key Analyses Performed

1. **Customer Behavior Analysis**
   - Shopping frequency patterns
   - Order timing and seasonality
   - Customer segmentation based on purchasing habits

2. **Product Analysis**
   - Most popular products and categories
   - Product reorder rates and patterns
   - Department-wise sales distribution

3. **Market Basket Analysis**
   - Product association and correlation
   - Shopping cart composition analysis
   - Cross-selling opportunities identification

## 📈 Key Findings

- **Shopping Time Patterns**: Most orders occur between 9:00 AM and 5:00 PM, with distinct peaks at 10:00 AM and 3:00 PM, indicating preferred shopping hours for grocery delivery
- **Weekly Shopping Behavior**: Customers place more orders at the beginning of the week (Sunday and Monday), with Sunday being the most popular shopping day
- **Reorder Frequency**: Most customers wait between 2-10 days between orders, with 7 days being the most common interval, indicating weekly grocery shopping habits
- **Subscription Patterns**: Notable spike at 30-day intervals suggests recurring monthly subscriptions, with additional smaller spikes at 14, 21, and 28 days for bi-weekly, tri-weekly, and monthly ordering cycles
- **Product Reorder Insights**: Produce and dairy comprise the most frequently reordered products, as perishable items naturally require regular replenishment
- **Cart Size Patterns**: Typical orders contain 5-6 items, with most orders ranging between 1-20 items total
- **First Cart Items**: Products most often placed in carts first are produce, dairy, and beverages (soda/water), potentially influenced by app design prioritizing popular items
- **Data Quality Observations**: Missing product names were isolated to department 21 (missing aisle) and aisle 100, handled by replacing with "unknown" values
- **Customer Loyalty Indicators**: High reorder rates for staple items like bananas and organic produce demonstrate consistent customer preferences and shopping habits

## 📁 Files in This Project

- `instacart_market_basket_analysis.ipynb` - Main analysis notebook
- `README.md` - Project documentation

## 🔗 Navigation

← [Back to Main Portfolio](../README.md)

---

**Part of the TripleTen Data Science Bootcamp Portfolio**