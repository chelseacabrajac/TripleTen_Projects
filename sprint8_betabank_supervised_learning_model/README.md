# Beta Bank Customer Churn Prediction Model

**Sprint 8 Project - TripleTen Data Science Bootcamp**

## 📋 Project Overview

This project develops a **Machine Learning Classification Model** to predict customer churn for Beta Bank. The bank has been experiencing a steady erosion of their customer base as clients gradually leave month after month. Since acquiring new customers is often more expensive than retaining existing ones, the goal is to build a predictive model that can identify customers likely to leave the bank, enabling proactive retention strategies to reduce losses and strengthen customer loyalty.

## 🎯 Objectives

- Develop a classification model to predict customer churn based on behavioral and contractual data
- Achieve minimum F1 score threshold of 59% on test dataset
- Compare multiple machine learning algorithms and optimize hyperparameters
- Implement proper train/validation/test split methodology with class imbalance handling
- Perform model validation and evaluate using both F1 score and AUC-ROC metrics
- Provide actionable business recommendations for customer retention deployment

## 🛠️ Technologies & Libraries Used

- **Python** - Primary programming language
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computations
- **Scikit-learn** - Machine learning algorithms and model evaluation
- **Matplotlib** - Data visualization
- **Jupyter Notebook** - Interactive development environment

### Machine Learning Algorithms
- **Logistic Regression** - Linear classification baseline
- **Decision Tree Classifier** - Tree-based interpretable model
- **Random Forest Classifier** - Ensemble method for improved accuracy

## 📊 Key Analyses Performed

### **Data Preparation & Methodology**
1. **Dataset Analysis**
   - Analyzed customer behavioral and contractual data from Beta Bank
   - Comprehensive data exploration and quality assessment
   - Feature engineering and preparation for machine learning
   - Target variable: customer churn indicator (stay vs leave)

2. **Data Splitting Strategy**
   - **Training Set**: 60% - Model training and learning
   - **Validation Set**: 20% - Hyperparameter tuning and model selection
   - **Test Set**: 20% - Final model evaluation and performance assessment

### **Class Imbalance Handling**

3. **Sampling Techniques Evaluation**
   - **Upsampling**: Increasing minority class (churned customers) samples
   - **Downsampling**: Reducing majority class (retained customers) samples
   - **Impact Analysis**: Compared model performance across sampling strategies

### **Model Development & Hyperparameter Optimization**

4. **Random Forest Classifier (Original Data)**
   - **Hyperparameters Tuned**: n_estimators, max_depth
   - **Best Configuration**: n_estimators=40, max_depth=15
   - **Validation Performance**: Baseline model assessment

5. **Random Forest Classifier (Upsampled Data)**
   - **Hyperparameters Tuned**: n_estimators, max_depth
   - **Optimization Strategy**: Systematic parameter search with balanced dataset
   - **Best Configuration**: n_estimators=90, max_depth=15
   - **Validation Performance**: Significant improvement with upsampling

6. **Random Forest Classifier (Downsampled Data)**
   - **Configuration**: Same hyperparameter optimization approach
   - **Performance Comparison**: Lower effectiveness compared to upsampling
   - **F1 Score**: 48.1% (below target threshold)

### **Model Evaluation & Validation**

7. **Performance Comparison**
   - **Best Performing Model**: Upsampled Random Forest Classifier
   - **F1 Score Achievement**: 61% (exceeds 59% threshold)
   - **Model Ranking**: Upsampled RF > Original RF > Downsampled RF

8. **Comprehensive Metrics Analysis**
   - **Accuracy**: 84.2%
   - **Precision**: 64.6% (prioritized for business value)
   - **Recall**: 57.8%
   - **AUC-ROC**: 85.3%
   - **Confusion Matrix**: [1438, 135], [180, 247]

9. **Threshold Optimization**
   - **Business-Focused Tuning**: Evaluated thresholds from 0.3 to 0.8
   - **Selected Threshold**: 0.5 (balances precision and business value)
   - **Strategic Decision**: Prioritized precision over recall for cost-effective retention campaigns

## 📈 Key Findings & Business Impact

- **Model Performance**: Successfully achieved 61% F1 score, exceeding the 59% business requirement
- **Algorithm Effectiveness**: Random Forest with upsampling proved most effective for handling class imbalance
- **Business Value**: Model correctly identifies churning customers with 64.6% precision, enabling targeted retention efforts
- **Cost Efficiency**: High precision reduces wasted resources on false positive retention campaigns
- **Deployment Readiness**: Strong AUC-ROC (85.3%) demonstrates excellent discriminatory power

## 🎯 Business Recommendations

### **Implementation Strategy**
1. **Deploy Upsampled Random Forest Model** in Beta Bank's customer relationship management system
2. **Focus on Precision-Driven Campaigns** targeting high-confidence churn predictions
3. **Implement Threshold Monitoring** to maintain optimal precision-recall balance
4. **Establish Continuous Retraining** pipeline to adapt to changing customer behaviors

### **Expected Business Benefits**
- **Reduced Customer Churn** through proactive identification of at-risk customers
- **Improved Resource Allocation** by focusing retention efforts on genuinely at-risk customers
- **Enhanced Customer Lifetime Value** through timely intervention strategies
- **Cost-Effective Retention Programs** with 64.6% precision reducing false positive costs

### **Strategic Considerations**
- **Precision Over Recall**: Model optimized for confident predictions rather than catching all churners
- **Resource Optimization**: Better to focus on customers you're confident about leaving
- **Campaign Effectiveness**: Targeted interventions on high-confidence predictions maximize ROI

## 📁 Files in This Project

- `sprint8_betabank_supervised_learning_model.ipynb` - Main analysis and model development notebook
- `README.md` - Project documentation

## 🔗 Navigation

← [Back to Main Portfolio](../README.md)

---

**Part of the TripleTen Data Science Bootcamp Portfolio**