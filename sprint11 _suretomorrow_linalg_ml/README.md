# SureTomorrow Insurance ML & Data Privacy

**Sprint 11 Project - TripleTen Data Science Bootcamp**

## 📋 Project Overview

This project demonstrates comprehensive **Machine Learning Applications with Linear Algebra and Data Privacy Protection** for SureTomorrow Insurance Company. The analysis combines multiple ML techniques including customer similarity analysis, classification, regression, and innovative data obfuscation methods. Using customer insurance data, the project addresses four critical business challenges: customer segmentation, benefit prediction, claims forecasting, and privacy-preserving analytics through linear algebraic transformations.

## 🎯 Objectives

- Implement k-Nearest Neighbors algorithm for customer similarity analysis and marketing applications
- Develop binary classification models to predict insurance benefit likelihood with imbalanced data handling
- Build custom linear regression implementation using linear algebra for claims volume prediction
- Design and validate privacy-preserving data obfuscation techniques using invertible matrix transformations
- Analyze the impact of feature scaling on distance-based vs. linear models
- Prove analytically that linear transformations preserve model performance while protecting data privacy
- Generate actionable business intelligence for insurance operations and customer management

## 🛠️ Technologies & Libraries Used

- **Python** - Primary programming language
- **Pandas** - Data manipulation and analysis
- **NumPy** - Linear algebra operations and matrix computations
- **Scikit-learn** - Machine learning algorithms and evaluation metrics
- **Seaborn** - Statistical data visualization
- **Jupyter Notebook** - Interactive development environment

### Advanced Techniques
- **Linear Algebra** - Matrix operations, inversions, and transformations
- **Custom ML Implementation** - Hand-built linear regression using analytical solutions
- **Privacy-Preserving Analytics** - Data obfuscation through invertible transformations
- **Distance Metrics** - Euclidean and Manhattan distance calculations

### Machine Learning Algorithms
- **k-Nearest Neighbors (k-NN)** - Customer similarity and classification
- **Linear Regression** - Claims volume prediction with analytical solutions
- **Dummy Classifiers** - Baseline performance evaluation

## 📊 Key Analyses Performed

### **Task 1: Customer Similarity Analysis**
1. **k-NN Implementation for Marketing**
   - Developed customer similarity search using k-Nearest Neighbors algorithm
   - Implemented custom `get_knn()` function with configurable distance metrics
   - Analyzed 4 feature combinations: gender, age, income, family_members
   - Compared Euclidean vs Manhattan distance metrics for similarity detection

2. **Feature Scaling Impact Analysis**
   - **Unscaled Data**: Income-dominated distance calculations due to scale differences
   - **MaxAbsScaler Application**: Balanced feature contribution to similarity metrics
   - **Key Finding**: Scaling essential for fair similarity calculations across diverse feature ranges
   - **Metric Comparison**: Manhattan and Euclidean distances produce similar results post-scaling

### **Task 2: Insurance Benefit Classification (Imbalanced Data)**
3. **Binary Classification Model Development**
   - **Target Variable**: Insurance benefits received (binary: 0/1)
   - **Class Distribution**: Highly imbalanced (~11% positive cases)
   - **Model Evaluation**: F1-score optimization for minority class detection
   - **k-NN Hyperparameter Tuning**: Systematic evaluation k=1 to k=10

4. **Scaling Impact on Classification Performance**
   - **Unscaled Performance**: F1=0.67 (k=1), rapidly declining with higher k
   - **Scaled Performance**: F1=0.95 (k=1), stable >0.90 across all k values
   - **Performance Gain**: 42% improvement in F1-score through proper scaling
   - **Model Robustness**: Scaled models less sensitive to k parameter selection

5. **Baseline Comparison with Dummy Models**
   - **Always Predict 0**: F1=0.00 (never detects positive cases)
   - **Random with Class Prevalence (~11%)**: F1≈0.12
   - **Random 50/50**: F1≈0.20
   - **Always Predict 1**: F1≈0.20
   - **Business Value**: k-NN model (F1=0.95) significantly outperforms all baselines

### **Task 3: Custom Linear Regression Implementation**
6. **Mathematical Foundation & Implementation**
   - **Analytical Solution**: $w = (X^T X)^{-1} X^T y$
   - **Custom Class**: `MyLinearRegression` with matrix operations
   - **Bias Term Handling**: Automatic addition of intercept column
   - **Performance Metrics**: RMSE and R² evaluation

7. **Scaling Invariance Analysis**
   - **Unscaled Model**: RMSE≈0.34, R²≈0.66
   - **Scaled Model**: RMSE≈0.34, R²≈0.66 (identical performance)
   - **Mathematical Proof**: Linear regression compensates for scaling through coefficient adjustment
   - **Prediction Difference**: <10⁻¹⁴ (floating-point precision only)

### **Task 4: Privacy-Preserving Data Obfuscation**
8. **Linear Transformation-Based Privacy Protection**
   - **Obfuscation Method**: $X' = X \times P$ (invertible matrix transformation)
   - **Privacy Mechanism**: Random invertible matrix P obscures original feature values
   - **Recoverability**: $X = X' \times P^{-1}$ (with knowledge of P)
   - **Security Analysis**: Original features unrecognizable without transformation matrix

9. **Analytical Proof of Model Invariance**
   - **Mathematical Derivation**: 
     - Original weights: $w = (X^T X)^{-1} X^T y$
     - Obfuscated weights: $w_P = P^{-1} w$
     - Predictions: $\hat{y}_P = (XP)w_P = Xw = \hat{y}$
   - **Performance Preservation**: RMSE and R² remain identical under transformation
   - **Privacy-Performance Trade-off**: Zero performance loss while achieving data protection

10. **Computational Validation**
    - **Implementation**: `LRWithObfuscation` class with optional privacy transformation
    - **Performance Comparison**: Original vs Obfuscated models show identical metrics
    - **Numerical Verification**: Prediction differences <10⁻¹² (rounding errors only)
    - **Business Application**: Secure data sharing without model quality degradation

## 📈 Key Findings & Technical Insights

- **Feature Scaling Critical for Distance-Based Models**: k-NN performance improved 42% (F1: 0.67→0.95) through proper scaling, while linear regression remained unaffected

- **Class Imbalance Handling**: Successfully addressed 11% minority class through F1-score optimization, achieving 4.75x improvement over random baseline performance

- **Custom Linear Algebra Implementation**: Demonstrated mastery of analytical solutions with matrix operations, achieving identical performance to scikit-learn implementations

- **Privacy-Performance Theorem**: Proved both analytically and computationally that invertible linear transformations preserve model accuracy while protecting sensitive data

- **Algorithm Selection Insights**: Distance-based algorithms require careful preprocessing, while linear models are naturally scale-invariant due to coefficient compensation

- **Business-Ready Solutions**: All four tasks address real insurance industry challenges with practical, deployable implementations

## 🔐 Privacy & Security Implications

### **Data Protection Mechanism**
- **Obfuscation Strength**: Original features (age, income, gender, family size) become uninterpretable combinations
- **Security Level**: Without matrix P, recovery is computationally infeasible for practical purposes
- **Compliance Ready**: Supports GDPR and other data protection regulations through anonymization

### **Model Integrity Preservation**
- **Zero Performance Loss**: Mathematical guarantee that predictive accuracy remains unchanged
- **Deployment Flexibility**: Models can operate on obfuscated data in cloud environments
- **Risk Mitigation**: Data breaches expose only transformed values, not personal information

## 🎯 Business Recommendations

### **Customer Similarity & Marketing (Task 1)**
**Implementation**: Deploy scaled k-NN system for customer segmentation
- **Marketing Applications**: Identify similar customers for targeted campaigns
- **Cross-selling Opportunities**: Recommend products based on similar customer profiles
- **Customer Service**: Provide personalized support based on behavioral similarities

### **Benefit Prediction & Risk Assessment (Task 2)**
**Implementation**: Deploy k-NN classifier (k=1, scaled features) for benefit likelihood prediction
- **Risk Management**: Identify high-probability claimants for proactive management
- **Premium Optimization**: Adjust pricing based on predicted benefit likelihood
- **Resource Allocation**: Allocate customer service resources based on predicted needs

### **Claims Volume Forecasting (Task 3)**
**Implementation**: Deploy linear regression model for benefit quantity prediction
- **Financial Planning**: Forecast total benefit payouts for budgeting
- **Capacity Planning**: Predict claim processing workload requirements
- **Product Development**: Design insurance products based on predicted usage patterns

### **Privacy-Preserving Analytics (Task 4)**
**Implementation**: Apply obfuscation framework for secure data operations
- **Data Sharing**: Enable secure collaboration with partners and vendors
- **Cloud Deployment**: Run analytics on public cloud with privacy protection
- **Regulatory Compliance**: Meet data protection requirements while maintaining insights

### **Expected Business Impact**
- **Customer Acquisition**: Improved targeting through similarity analysis
- **Risk Management**: Proactive identification of high-risk customers
- **Operational Efficiency**: Accurate forecasting enables better resource planning
- **Competitive Advantage**: Privacy-preserving analytics enables secure innovation
- **Compliance Assurance**: Data protection capabilities support regulatory requirements

## 📁 Files in This Project

- `sprint11_suretomorrow_linalg_ml.ipynb` - Main analysis and modeling notebook
- `README.md` - Project documentation

## 🔗 Navigation

← [Back to Main Portfolio](../README.md)

---

**Part of the TripleTen Data Science Bootcamp Portfolio**