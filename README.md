
## 🚀 **Project Overview: Renewal of Insurance Policies**  

### 📌 **Objective**  
The goal of this project is to predict whether customers will renew their insurance policies next year based on various demographic and policy-related factors.  

### 🗂 **Data Summary**  
- **Total Observations:** 74,200 (after preprocessing: 51,945)  
- **Number of Features:** 37  
- **Target Variable:** `renew_next_year` (Binary: Renewed/Not Renewed)  

---

## 🛠 **Key Steps and Approach**  

### 1. **Data Preprocessing & Feature Engineering**  
- Dropped irrelevant columns and handled missing values.  
- Analyzed correlations to identify key variables such as:  
  - **Highly Correlated Features:** `renew_next_month`, `age`, `tenure`, `have_house_insurance`.  
- Applied **Lasso Regression** for feature selection, improving interpretability and achieving an accuracy of **89%** with selected features.  

### 2. **Model Selection & Results**  
- Implemented **Logistic Regression**, achieving a solid **88% accuracy** in predicting policy renewals.  
- Key features considered: `tenure, age, no_of_covers, renew_next_month, have_child_insurance, have_house_insurance`.  
- Performance metrics:  
  - **Precision:** 88%  
  - **Recall:** 100%  
  - **F1-score:** 94%  
- However, the model struggled to accurately predict non-renewals, indicating room for improvement.  

### 3. **Model Improvement Efforts**  
- Addressing class imbalance using advanced techniques such as:  
  - Oversampling (SMOTE)  
  - Ensemble methods (Random Forest, XGBoost)  
  - Feature engineering to enhance variable effectiveness.  

---

## 📊 **Key Insights & Findings**  
- **Renewal Trends:**  
  - Majority (88.16%) of customers tend to renew their policies.  
  - Renewal rates show a **slight decrease over time**, indicating potential customer churn.  
- **Stability Testing:**  
  - Conducted statistical tests (Chi-Square) revealing that the observed renewal patterns are **not consistent across time periods**, suggesting dynamic factors influencing renewal decisions.  

---

## 🔧 **Tools & Technologies Used**  
- **Programming Languages:** Python, R  
- **Machine Learning Algorithms:** Logistic Regression, Lasso Regression, Decision Trees  
- **Libraries:** Pandas, NumPy, scikit-learn, Matplotlib, Seaborn  
- **Statistical Tests:** Chi-Square test for pattern stability analysis  
- **AI Assistance:** Leveraged ChatGPT for insights, code optimization, and exploratory analysis.  

---

## 📚 **Lessons Learned**  
- Importance of feature selection in improving model performance.  
- Handling class imbalance is critical for accurate predictions.  
- Statistical analysis is key to understanding business trends and seasonality.  

---

## 🌟 **Future Enhancements**  
- Explore deep learning techniques for better prediction accuracy.  
- Implement automated feature engineering pipelines.  
- Deploy the model as a web-based dashboard for real-time policy renewal monitoring.  

