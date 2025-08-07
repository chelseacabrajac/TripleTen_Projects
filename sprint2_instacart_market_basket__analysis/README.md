# Instacart Market Basket Analysis

**Sprint 2 Project - TripleTen Data Science Bootcamp**

## 📋 Project Overview

This project demonstrates comprehensive **Instacart Market Basket Analysis** through systematic data cleaning, exploratory data analysis, and customer behavior insights using real grocery shopping data. The analysis covers data preprocessing, statistical exploration across multiple datasets, and in-depth investigation of shopping patterns, product popularity, and customer ordering behaviors.

## 🎯 Objectives

- Master data cleaning techniques for multi-table relational datasets
- Perform systematic exploratory data analysis to uncover shopping patterns
- Analyze customer behavior across temporal dimensions (hourly, daily, weekly)
- Investigate product popularity, reorder patterns, and cart composition
- Apply statistical methods to extract actionable business insights from transactional data
- Develop proficiency in merging datasets and aggregating complex data structures

## 🛠️ Technologies & Libraries Used

- **Python** - Primary programming language
- **Pandas** - Data manipulation, merging, and analysis
- **Matplotlib** - Data visualization and statistical plotting
- **Jupyter Notebook** - Interactive development environment

## 📊 Key Analyses Performed

### **Data Cleaning & Preprocessing**
1. **Missing Values Analysis & Treatment**
   - Identified missing product names in aisle 100/department 21 (missing category)
   - Replaced missing product names with 'unknown' values
   - Analyzed missing `days_since_prior_order` for first-time customers (kept as NaN)
   - Handled missing `add_to_cart_order` for items 65+ with code value 999

2. **Duplicate Detection & Removal**
   - Removed 15 duplicate orders with identical timestamps
   - Eliminated duplicate product names using case-insensitive comparison
   - Cleaned product catalog maintaining unique identifiers

### **Easy Level Analyses (A1-A4)**
3. **Data Validation & Temporal Analysis**
   - Verified sensible ranges for `order_hour_of_day` (0-23) and `order_dow` (0-6)
   - **Shopping Time Patterns**: Peak ordering times 9 AM-5 PM with peaks at 10 AM and 3 PM
   - **Weekly Patterns**: Higher order volume on weekends and Mondays (Sunday = day 0)
   - **Reorder Intervals**: Most common wait time is 7 days with notable 30-day subscription spike

### **Medium Level Analyses (B1-B3)**
4. **Advanced Temporal & Customer Analysis**
   - **Wednesday vs Saturday**: Identified lunch-hour dip (11 AM-1 PM) on weekdays absent on weekends
   - **Customer Order Distribution**: Most customers place 1-10 orders with sharp decline after first order
   - **Product Popularity**: Top 20 products dominated by produce and dairy items

### **Hard Level Analyses (C1-C5)**
5. **In-depth Behavioral & Cart Analysis**
   - **Order Size Distribution**: Typical orders contain 5-6 items, most orders 1-20 items
   - **Reorder Analysis**: Produce and dairy most frequently reordered (perishable goods pattern)
   - **Customer Reorder Rates**: Individual customer reorder proportion analysis
   - **Cart Composition**: First-added items are produce, dairy, and beverages (app design influence)

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