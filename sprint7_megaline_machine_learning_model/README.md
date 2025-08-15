# Megaline Mobile Plan Recommendation Model

**Sprint 7 Project - TripleTen Data Science Bootcamp**

## 📋 Project Overview

This project develops a **Machine Learning Classification Model** to recommend optimal mobile plans for Megaline subscribers. The company discovered that many customers are still using legacy plans and wants to transition them to newer, more suitable options: Smart or Ultra plans. Using behavioral data from subscribers who have already switched, the goal is to build a predictive model that can automatically recommend the best plan based on usage patterns.

## 🎯 Objectives

- Develop a classification model to recommend Smart or Ultra plans based on subscriber behavior
- Achieve minimum accuracy threshold of 75% on test dataset
- Compare multiple machine learning algorithms and optimize hyperparameters
- Implement proper train/validation/test split methodology
- Perform model validation and sanity checks to ensure reliability
- Provide actionable business recommendations for plan recommendation deployment

## 🛠️ Technologies & Libraries Used

- **Python** - Primary programming language
- **Pandas** - Data manipulation and analysis
- **Scikit-learn** - Machine learning algorithms and model evaluation
- **Matplotlib** - Data visualization
- **Jupyter Notebook** - Interactive development environment

### Machine Learning Algorithms
- **Decision Tree Classifier** - Baseline tree-based model
- **Random Forest Classifier** - Ensemble method for improved accuracy
- **Logistic Regression** - Linear classification approach

## 📊 Key Analyses Performed

### **Data Preparation & Methodology**
1. **Dataset Analysis**
   - Analyzed subscriber behavioral data from users who switched to new plans
   - No data preprocessing required (completed in previous project)
   - Feature extraction: calls, minutes, messages, megabytes usage
   - Target variable: plan recommendation (Smart vs Ultra)

2. **Data Splitting Strategy**
   - **Training Set**: 60% - Model training and learning
   - **Validation Set**: 20% - Hyperparameter tuning and model selection
   - **Test Set**: 20% - Final model evaluation and accuracy assessment

### **Model Development & Hyperparameter Optimization**

3. **Decision Tree Classifier**
   - **Hyperparameters Tuned**: max_depth, min_samples_split, min_samples_leaf
   - **Optimization Process**: Systematic grid search across parameter ranges
   - **Best Configuration**: max_depth=7, min_samples_split=55, min_samples_leaf=1
   - **Validation Accuracy**: ~80%

4. **Random Forest Classifier**
   - **Hyperparameters Tuned**: n_estimators, max_depth, min_samples_split, min_samples_leaf
   - **Optimization Strategy**: Sequential parameter tuning for optimal performance
   - **Best Configuration**: n_estimators=150, max_depth=None, min_samples_split=2, min_samples_leaf=1
   - **Validation Accuracy**: ~82%

5. **Logistic Regression**
   - **Configuration**: solver='liblinear' for binary classification
   - **Performance**: Baseline linear model comparison
   - **Validation Accuracy**: ~72%

### **Model Evaluation & Validation**

6. **Performance Comparison**
   - **Best Performing Model**: Random Forest Classifier
   - **Test Accuracy Achievement**: 78.85% (exceeds 75% threshold)
   - **Model Ranking**: Random Forest > Decision Tree > Logistic Regression

7. **Sanity Check Analysis**
   - **Training vs Test Accuracy**: 83% vs 79% (slight overfitting, acceptable)
   - **Prediction Distribution**: Closely matches true label distribution
   - **Model Reliability**: Consistent performance across validation and test sets

## 📈 Key Findings & Business Impact

- **Model Performance**: Successfully achieved 78.85% accuracy, exceeding the 75% business requirement
- **Algorithm Effectiveness**: Random Forest proved most effective for this classification task, handling feature interactions better than simpler models
- **Business Value**: Model correctly recommends plans ~8 out of 10 times, significantly improving customer plan matching
- **Deployment Readiness**: Model demonstrates good generalization with minimal overfitting

## 🎯 Business Recommendations

### **Implementation Strategy**
1. **Deploy Random Forest Model** in Megaline's customer service and self-service systems
2. **Monitor Performance** continuously and retrain if accuracy drops below 75%
3. **Collect Additional Features** (roaming usage, streaming patterns) to enhance prediction power
4. **Balance Training Data** if Smart plan dominance creates prediction bias

### **Expected Business Benefits**
- **Reduced Customer Churn** through better plan-customer matching
- **Increased Plan Adoption** of newer Smart and Ultra offerings
- **Improved Customer Satisfaction** by avoiding unsuitable plan recommendations
- **Enhanced Customer Lifetime Value** through optimized service delivery

## 📁 Files in This Project

- `megaline_machine_learning_model.ipynb` - Main analysis and model development notebook
- `README.md` - Project documentation

## 🔗 Navigation

← [Back to Main Portfolio](../README.md)

---

**Part of the TripleTen Data Science Bootcamp Portfolio**
