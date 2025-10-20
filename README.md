# ❤️ Cardiovascular Disease Risk Analysis  
*Comparing logistic regression and random forest models to predict cardiovascular outcomes*


[![Substack](https://img.shields.io/badge/Read_on-Substack-orange?logo=substack)](https://danliontario.substack.com/p/predicting-cardiovascular-disease)  
[![Portfolio](https://img.shields.io/badge/View-Portfolio-blue?logo=react)](https://dlport.web.app/)  
--- 

## 📖 Project Overview  

**Cardiovascular disease (CVD)** remains one of the leading causes of mortality worldwide.  
This project analyzes a **70,000-participant clinical dataset** to understand how **lifestyle and physiological variables** — such as **age, BMI, blood pressure, and cholesterol** — predict cardiovascular outcomes.  

Two modeling paradigms are compared:  
- **Classical statistical modeling:** Logistic regression and interaction effects  
- **Machine learning:** Random forest classifier  

The study balances **interpretability vs. predictive accuracy**, offering a data-driven framework for early risk detection.  
---

## 🧪 Methods  

- **Tools:** R (`tidyverse`, `caret`, `randomForest`, `marginaleffects`, `pROC`)  
- **Models:** Logistic Regression, Interaction Model (Age × BMI × Cholesterol), Random Forest  
- **Dataset:** 70,000 records with 11 clinical and lifestyle variables  
- **Process:** Data cleaning, feature engineering, model training, AUC evaluation, and variable importance ranking  
--- 
## 📊 Key Findings

**Top Predictors:**
- Systolic blood pressure (ap_hi)
- Cholesterol level
- Age
- BMI

**Age × BMI Interaction:**
- Risk increases nonlinearly with both age and BMI.
- BMI has a stronger effect at younger ages but saturates by ~65 years.

**Gender Effect:**
- Men show higher risk across all BMI levels, with the gap widening above BMI ≈ 30.

**Model Comparison:**
- Model		Strength
- Logistic Regression	AUC	Accuracy: 0.72	Strength: 0.70|Interpretable and robust
- Interaction Model	AUC	Accuracy: 0.71	Strength: 0.69|Captures nonlinearities
- Random Forest	AUC	Accuracy: 0.75	Strength: 0.73|Best predictive accuracy

--- 
