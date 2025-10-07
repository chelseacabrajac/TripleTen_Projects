# Gold Recovery Prediction Model

**Sprint 10 Project - TripleTen Data Science Bootcamp**

## 📋 Project Overview

This project develops a comprehensive **Machine Learning Regression Model** to predict gold recovery efficiency at different stages of an industrial flotation process for a mining operation. The analysis combines rigorous data validation, advanced preprocessing techniques, and predictive modeling to optimize gold extraction processes. Using geological and process data from multiple purification stages, the goal is to build accurate models that can predict recovery rates for both rougher and final processing stages.

## 🎯 Objectives

- Validate recovery calculation formulas against actual dataset values for data integrity
- Implement comprehensive data preprocessing including outlier removal and missing value handling
- Analyze metal concentration patterns across different purification stages
- Develop regression models to predict gold recovery at rougher and final stages
- Compare model performance using industry-appropriate evaluation metrics (sMAPE)
- Generate actionable predictions for real-world mining operations
- Ensure model reliability through cross-validation and proper train/test methodology

## 🛠️ Technologies & Libraries Used

- **Python** - Primary programming language
- **Pandas** - Data manipulation and preprocessing
- **NumPy** - Numerical computations and statistical operations
- **Scikit-learn** - Machine learning algorithms and model evaluation
- **Matplotlib** - Data visualization and distribution analysis
- **Jupyter Notebook** - Interactive development environment

### Machine Learning Algorithms
- **Linear Regression** - Baseline regression model
- **Random Forest Regressor** - Advanced ensemble method for non-linear relationships

### Statistical Techniques
- **Cross-Validation** - Model performance validation
- **sMAPE (Symmetric Mean Absolute Percentage Error)** - Industry-specific evaluation metric
- **Outlier Detection & Removal** - Data quality enhancement

## 📊 Key Analyses Performed

### **Data Validation & Quality Assurance**
1. **Recovery Formula Validation**
   - Implemented recovery calculation: `(C * (F-T)) / (F * (C-T)) * 100`
   - Validated against dataset values with MAE of 9.30 × 10⁻¹⁵ (essentially perfect match)
   - Filtered invalid rows with problematic concentration values
   - Retained 14,287 valid rows out of 16,860 total for reliable analysis

2. **Data Integrity Assessment**
   - Identified missing target variables and process output columns in test set
   - Prevented data leakage by excluding post-process measurements from training
   - Ensured model uses only pre-process operational features (52 common features)
   - Validated temporal consistency and removed duplicate entries

### **Comprehensive Data Preprocessing**
3. **Missing Value Treatment**
   - Applied median imputation for numerical features across all datasets
   - Used forward-fill method for categorical variables
   - Maintained consistency between train, test, and full datasets
   - Preserved target variable integrity by excluding from imputation

4. **Outlier Detection & Removal**
   - Implemented percentile-based outlier removal (1st and 99th percentiles)
   - Applied to all numerical columns for data quality enhancement
   - Reduced training set from ~16K to 5,831 samples for cleaner modeling
   - Balanced data quality vs. quantity for optimal model performance

### **Exploratory Data Analysis & Process Insights**
5. **Metal Concentration Analysis**
   - **Gold (Au)**: Concentrations increase through purification stages (feed → rougher → final)
   - **Silver (Ag)**: Concentrations decrease during flotation process
   - **Lead (Pb)**: Remains relatively stable throughout processing stages
   - **Process Validation**: Confirms flotation system optimized for gold recovery

6. **Feed Particle Size Distribution**
   - Analyzed particle size consistency between train and test sets
   - Confirmed similar distributions (0-100 µm range) ensuring model reliability
   - Validated optimal particle size range for flotation efficiency
   - Established process monitoring baseline for operational control

7. **Stage-wise Concentration Profiles**
   - Input stage: Raw feed characteristics and composition
   - Rougher stage: Initial separation and concentration
   - Final stage: Purified concentrate with maximized gold content
   - Primary cleaner: Intermediate purification with reduced impurities

### **Advanced Predictive Modeling**
8. **Model Development & Hyperparameter Optimization**
   - **Random Forest Regressor**: n_estimators=100, max_depth=10, optimized parameters
   - **Linear Regression**: Baseline comparison model
   - **Cross-Validation**: 5-fold validation for robust performance assessment
   - **Feature Selection**: 52 common input features to prevent data leakage

9. **Performance Evaluation using sMAPE**
   - **Combined Metric**: 25% rougher recovery + 75% final recovery (industry weighting)
   - **Random Forest Results**: Rougher sMAPE=7.23%, Final sMAPE=4.50%, Combined=5.19%
   - **Linear Regression Results**: Rougher sMAPE=8.53%, Final sMAPE=5.70%, Combined=6.41%
   - **Model Selection**: Random Forest achieved 19% improvement over Linear Regression

### **Real-world Prediction & Deployment Readiness**
10. **Test Set Predictions**
    - **Rougher Recovery Range**: 46-76% (higher variability reflecting initial separation)
    - **Final Recovery Range**: 54-63% (stable, consistent purification outcomes)
    - **Prediction Validation**: Results align with expected process behavior
    - **Deployment Ready**: Model trained only on pre-process features for real-time application

## 📈 Key Findings & Process Intelligence

- **Data Quality Excellence**: Recovery formula validation confirmed perfect alignment with dataset, ensuring mathematical correctness and data integrity

- **Process Understanding**: Metal concentration analysis revealed flotation system optimized specifically for gold recovery, with silver reduction and lead stability indicating targeted separation chemistry

- **Robust Preprocessing**: Strategic outlier removal (retaining 5,831 samples) balanced data quality with sufficient training volume for reliable modeling

- **Model Superiority**: Random Forest significantly outperformed Linear Regression (5.19% vs 6.41% combined sMAPE), capturing non-linear relationships in gold recovery process

- **Industry-Relevant Accuracy**: Combined sMAPE of 5.19% provides excellent predictive performance for real-world process optimization and operational decision-making

- **Stage-Specific Insights**: Rougher stage predictions more variable (reflecting upstream ore variability), final stage more stable (controlled purification environment)

## 🎯 Business Recommendations

### **Operational Deployment**
**Recommended Model: Random Forest Regressor**
- **Performance**: 5.19% combined sMAPE (exceeds industry standards)
- **Reliability**: Robust cross-validation performance with 19% improvement over baseline
- **Applicability**: Trained on pre-process features for real-time operational use

### **Implementation Strategy**
1. **Deploy for Real-time Monitoring** - Integrate model into process control systems for continuous recovery prediction
2. **Process Optimization** - Use predictions to adjust operational parameters proactively
3. **Quality Control** - Monitor deviations from expected recovery ranges for early intervention
4. **Yield Forecasting** - Improve production planning with accurate recovery predictions

### **Expected Business Impact**
- **Improved Recovery Rates** through data-driven process optimization
- **Reduced Operating Costs** via proactive parameter adjustment and waste minimization
- **Enhanced Production Planning** with reliable yield forecasting capabilities
- **Risk Mitigation** through early detection of suboptimal operating conditions
- **Competitive Advantage** via advanced analytics-driven mining operations

### **Continuous Improvement Opportunities**
- **Feature Engineering** - Incorporate additional process variables for enhanced accuracy
- **Model Retraining** - Regular updates with new operational data
- **Advanced Algorithms** - Explore gradient boosting and neural networks for further improvement
- **Multi-objective Optimization** - Balance recovery rate with energy consumption and reagent costs

## 📁 Files in This Project

- `sprint10_gold_recovery_prediction.ipynb` - Main analysis and modeling notebook
- `README.md` - Project documentation

## 🔗 Navigation

← [Back to Main Portfolio](../README.md)

---

**Part of the TripleTen Data Science Bootcamp Portfolio**