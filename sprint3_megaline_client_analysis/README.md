# Megaline Mobile Plan Analysis

**Sprint 3 Project - TripleTen Data Science Bootcamp**

## 📋 Project Overview

This project demonstrates comprehensive **Mobile Service Usage Analysis and Statistical Hypothesis Testing** using real telecom data from Megaline. The analysis involves systematic data preprocessing across multiple datasets, revenue calculation methodology development, usage pattern analysis, and rigorous statistical testing to determine which subscription plan generates more revenue and identify regional differences in customer behavior.

## 🎯 Objectives

- Master multi-dataset integration and preprocessing for telecom usage analysis
- Develop revenue calculation methodology based on complex plan structures and overage charges
- Conduct comprehensive exploratory data analysis of customer usage patterns
- Apply statistical hypothesis testing to validate business assumptions about plan performance
- Perform regional analysis to identify geographic differences in customer behavior
- Generate data-driven business recommendations for marketing and plan optimization

## 🛠️ Technologies & Libraries Used

- **Python** - Primary programming language
- **Pandas** - Data manipulation, merging, and aggregation
- **NumPy** - Numerical computations and data transformations
- **SciPy** - Statistical hypothesis testing (t-tests)
- **Matplotlib** - Data visualization and statistical plotting
- **Jupyter Notebook** - Interactive development environment

## 📊 Key Analyses Performed

### **Data Preprocessing & Integration**
1. **Multi-Dataset Cleaning**
   - **Plans Data**: Corrected GB measurements and standardized column naming
   - **Users Data**: Fixed data types, added regional classification (NY-NJ vs Other)
   - **Calls Data**: Rounded call durations per Megaline billing practices, added monthly aggregation
   - **Messages Data**: Standardized date formats and user ID types
   - **Internet Data**: Converted MB to GB usage, implemented monthly grouping

2. **Data Integration & Aggregation**
   - Merged five separate datasets into comprehensive monthly user profiles
   - Created monthly usage summaries per user for calls, messages, and internet
   - Developed complex revenue calculation function incorporating plan limits and overage charges

### **Usage Pattern Analysis**
3. **Call Behavior Analysis**
   - Ultimate plan shows more consistent monthly usage patterns
   - Surf plan users average 6000-8000 minutes yearly with notable business user outliers
   - Identified potential business users through exceptionally high usage patterns

4. **Messaging Pattern Analysis**
   - Similar usage patterns across both plans (not a plan differentiator)
   - Most users send few messages monthly; heavy users reach 20,000+ messages
   - No significant plan-based behavioral differences

5. **Internet Usage Analysis**
   - **Clear Plan Differentiation**: Ultimate users consume 3000-5000+ GB range
   - **Plan Justification**: Surf users cluster in 0-2000 GB range
   - **Customer Self-Selection**: Users choose plans matching their actual usage patterns

### **Revenue Analysis & Business Intelligence**
6. **Plan Performance Comparison**
   - Surf plan generates more total revenue (339 users vs 161 Ultimate users)
   - Revenue advantage through overage charges despite lower base price
   - Right-skewed revenue distribution with high-revenue users (15,000-20,000 range) in Surf plan

7. **Regional Analysis**
   - NY-NJ users (80) vs Other regions (420) revenue comparison
   - Despite smaller user base, NY-NJ shows different revenue patterns

### **Statistical Hypothesis Testing**
8. **Plan Revenue Hypothesis Testing**
   - **H₀**: Equal average revenue between plans
   - **H₁**: Different average revenue between plans
   - **Result**: Rejected H₀ (p-value = 0.018 < α = 0.05)

9. **Regional Revenue Hypothesis Testing**
   - **H₀**: Equal revenue between NY-NJ and Other regions
   - **H₁**: Different revenue between regions  
   - **Result**: Rejected H₀ (p-value = 0.014 < α = 0.05)

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
