# OilyGiant Oil Well Location Analysis

**Sprint 9 Project - TripleTen Data Science Bootcamp**

## 📋 Project Overview

This project demonstrates comprehensive **Business Analytics and Risk Assessment** using machine learning to identify the most profitable location for OilyGiant Mining Company's new oil well development. The analysis combines predictive modeling with advanced statistical techniques including bootstrapping and confidence interval analysis to evaluate three potential regions, balancing profit potential against investment risk for data-driven decision making.

## 🎯 Objectives

- Build predictive models to estimate oil reserves across three geographical regions
- Apply statistical simulation techniques to assess profitability and investment risk
- Implement bootstrapping methodology to quantify uncertainty in profit projections
- Calculate confidence intervals and risk metrics for comprehensive investment analysis
- Provide data-driven recommendations for optimal well location selection
- Balance profit maximization with risk minimization for sustainable business growth

## 🛠️ Technologies & Libraries Used

- **Python** - Primary programming language
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computations and statistical operations
- **Scikit-learn** - Machine learning modeling and validation
- **Jupyter Notebook** - Interactive development environment

### Statistical & ML Techniques
- **Linear Regression** - Reserve prediction modeling
- **Bootstrapping** - Risk assessment and uncertainty quantification
- **Monte Carlo Simulation** - Profit distribution analysis

## 📊 Key Analyses Performed

### **Data Preprocessing & Model Development**
1. **Multi-Region Dataset Analysis**
   - Loaded and analyzed geological data from three distinct regions
   - Standardized data types and formats across all datasets
   - Feature engineering for geological characteristics (f0, f1, f2 parameters)
   - Target variable: oil reserves in thousand barrels

2. **Predictive Model Development**
   - **Algorithm**: Linear Regression for reserve estimation
   - **Train/Validation Split**: 75%/25% for each region
   - **Model Evaluation**: RMSE (Root Mean Square Error) for prediction accuracy
   - **Cross-Region Comparison**: Consistent methodology across all three regions

### **Business Parameter Definition & Breakeven Analysis**
3. **Investment Framework Setup**
   - **Total Budget**: $100,000,000 USD
   - **Wells to Explore**: 500 per region
   - **Wells to Develop**: Top 200 performing wells
   - **Revenue per Unit**: $4,500 USD per thousand barrels
   - **Cost per Well**: $500,000 USD per developed well
   - **Breakeven Threshold**: 111.11 thousand barrels per well

4. **Initial Profitability Assessment**
   - Region 1 Mean Predicted Reserves: 92.59 thousand barrels
   - Region 2 Mean Predicted Reserves: 68.73 thousand barrels  
   - Region 3 Mean Predicted Reserves: 95.00 thousand barrels
   - **Critical Finding**: All regions below breakeven threshold on average

### **Advanced Risk Analysis & Statistical Simulation**
5. **Top Well Selection Strategy**
   - Implemented profit calculation for top 200 wells per region
   - **Region 1**: $6,790,689 profit from top wells
   - **Region 2**: $7,794,799 profit from top wells (highest)
   - **Region 3**: $4,399,901 profit from top wells

6. **Bootstrap Simulation Analysis (1000 iterations)**
   - **Monte Carlo Method**: Random sampling with replacement
   - **Confidence Intervals**: 95% CI for profit projections
   - **Risk Quantification**: Probability of loss calculation
   - **Statistical Validation**: Robust uncertainty assessment

### **Risk Assessment & Investment Decision Framework**
7. **Comprehensive Risk-Return Analysis**
   
   **Region 1 Performance:**
   - Average Profit: $3,960,000
   - 95% CI: [-$1,070,000, $8,820,000]
   - Risk of Loss: 4.9%
   
   **Region 2 Performance:**
   - Average Profit: $4,510,000 (highest)
   - 95% CI: [$324,148, $8,520,000] (entirely positive)
   - Risk of Loss: 1.6% (lowest)
   
   **Region 3 Performance:**
   - Average Profit: $3,980,000
   - 95% CI: [-$1,470,000, $9,020,000]
   - Risk of Loss: 8.3% (highest)

8. **Investment Criteria & Final Selection**
   - **Risk Threshold**: <2.5% probability of loss
   - **Qualifying Region**: Only Region 2 meets risk criteria
   - **Downside Protection**: Region 2 shows positive returns even in worst-case scenarios
   - **Volatility Analysis**: Region 2 demonstrates most consistent performance

## 📈 Key Findings & Business Intelligence

- **Model Performance**: Linear regression models successfully predicted oil reserves with reasonable accuracy across all regions

- **Breakeven Challenge**: All regions showed average reserves below the 111.11 thousand barrel breakeven threshold, highlighting the importance of selective well development

- **Top Well Strategy**: Focusing on the top 200 wells (out of 500 explored) transforms unprofitable averages into profitable investments

- **Regional Superiority**: Region 2 demonstrates superior risk-adjusted returns with highest average profit ($4.51M) and lowest loss probability (1.6%)

- **Risk Quantification**: Bootstrap analysis revealed Region 2 as the only region with <2.5% risk of loss, providing crucial downside protection

- **Investment Confidence**: Region 2's 95% confidence interval remains entirely positive ($324K - $8.52M), ensuring profitability even in adverse scenarios

## 🎯 Business Recommendations

### **Strategic Investment Decision**
**Recommended Location: Region 2**
- **Expected Return**: $4,457,966 average profit
- **Risk Profile**: 1.6% probability of loss (meets <2.5% threshold)
- **Confidence Range**: $324,148 - $8,520,000 (95% CI)
- **Competitive Advantage**: Highest profit with lowest risk

### **Implementation Strategy**
1. **Proceed with Region 2 Development** - Deploy full $100M budget for maximum returns
2. **Implement Selective Development** - Focus on top 200 wells out of 500 explored
3. **Monitor Performance Metrics** - Track actual vs. predicted reserves for model refinement
4. **Risk Management** - Maintain contingency planning despite low loss probability

### **Expected Business Impact**
- **ROI Optimization**: 4.5% average return on $100M investment
- **Risk Mitigation**: 98.4% probability of positive returns
- **Market Positioning**: Data-driven approach provides competitive advantage
- **Scalability**: Proven methodology applicable to future site selection

## 📁 Files in This Project

- `sprint9_oilygiant_business_ml.ipynb` - Main analysis and modeling notebook
- `README.md` - Project documentation

## 🔗 Navigation

← [Back to Main Portfolio](../README.md)

---

**Part of the TripleTen Data Science Bootcamp Portfolio**