# Megaline Mobile Plan Analysis

**Sprint 3 Project - TripleTen Data Science Bootcamp**

## 📋 Project Overview

This project focuses on **Statistical Hypothesis Testing** using mobile service usage data from Megaline. The analysis compares different subscription plans to determine their performance and provides data-driven recommendations for plan optimization.

## 🎯 Objectives

- Analyze mobile service usage data to compare different subscription plans
- Conduct rigorous statistical hypothesis testing to determine plan performance
- Provide data-driven recommendations for mobile plan optimization
- Apply advanced statistical methods to validate business assumptions

## 🛠️ Technologies & Libraries Used

- **Python** - Primary programming language
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computations
- **SciPy** - Statistical hypothesis testing
- **Matplotlib** - Data visualization
- **Seaborn** - Statistical data visualization
- **Statsmodels** - Advanced statistical modeling
- **Jupyter Notebook** - Interactive development environment

## 📊 Key Analyses Performed

1. **Usage Pattern Analysis**
   - Call duration and frequency patterns
   - Data usage across different plans
   - SMS usage behavior analysis

2. **Plan Performance Comparison**
   - Revenue analysis by plan type
   - Customer satisfaction metrics
   - Usage vs. plan limits analysis

3. **Statistical Hypothesis Testing**
   - T-tests for plan comparison
   - Chi-square tests for categorical relationships
   - ANOVA for multiple group comparisons

## 📈 Key Findings

- **Revenue Performance**: Surf plan generates more revenue for Megaline overall, with 339 Surf users vs 161 Ultimate users, creating revenue advantage through overage charges despite lower base price
- **Plan Selection Patterns**: Users choose plans based on data usage needs - Ultimate plan users are heavier internet consumers (3000-5000+ GB range) while Surf users cluster in 0-2000 GB range
- **Statistical Hypothesis Testing - Plan Revenue**: Rejected null hypothesis that both plans generate equal average revenue (p-value = 0.018 < α = 0.05), confirming significant revenue difference between plans
- **Regional Revenue Analysis**: Rejected null hypothesis for NY-NJ vs Other regions revenue equality (p-value = 0.014 < α = 0.05), despite NY-NJ having fewer users (80 vs 420)
- **Call Usage Patterns**: Ultimate plan shows more consistent monthly call duration, while Surf plan users average 6000-8000 minutes yearly with notable outliers suggesting business users
- **Messaging Behavior**: Both plans show similar messaging patterns - most users send few messages monthly, with heavy users reaching 20,000+ messages, indicating messaging is not a plan differentiator
- **Internet Usage as Key Differentiator**: Clear plan justification exists - Ultimate users consume significantly more data, demonstrating customers choose plans matching their usage patterns
- **Revenue Distribution**: Both plans show right-skewed revenue distributions with Surf having more users in low revenue ranges, while some high-revenue users (15,000-20,000 range) appear only in Surf plan
- **Business Recommendations**: Target Surf plan marketing toward businesses and older demographics who prioritize voice communication, capitalizing on overage revenue from additional minutes

## 📁 Files in This Project

- `megaline_client_analysis.ipynb` - Main analysis notebook
- `README.md` - Project documentation

## 🔗 Navigation

← [Back to Main Portfolio](../README.md)

---

**Part of the TripleTen Data Science Bootcamp Portfolio**
