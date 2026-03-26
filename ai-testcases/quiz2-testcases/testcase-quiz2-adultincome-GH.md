# AI Testcase

### 1. TC-identifier:
Gage-Hulbert-Adult-Income

### 2. TC-name:
Adult Income Classification Explainability Test

### 3. TC-objective:
Determine if an AI model trained with the Adult Income dataset produces accurate binary income classification (<=50K vs >50K) and provides meaningful explanations using SHAP, LIME, and EBM explanation methods.

### 4. TC-input:
- Adult Income dataset (https://archive.ics.uci.edu/ml/machine-learning-databases/adult/adult.data)
- Models: Logistic Regression (whitebox), Explainable Boosting Machine (EBM)
- Explanation methods: SHAP (global + local), LIME (local), EBM global and local explain

### 5. TC-reference-output:
- Logistic Regression Accuracy: ~0.83
- EBM Accuracy: ~0.87
- Top features identified by SHAP and EBM: education_num, capital_gain, marital_status, hours_per_week
- EBM shape function for capital_gain shows a non-linear jump at higher values
- SHAP and LIME agree on top 3 features for individual predictions

### 6. TC-harm-risk-info:
- HC1-incorrect-info: Misclassifying income could introduce bias in real-world applications like loan approvals or financial services
- HC3-unstable-extrauserinfo: Dataset includes sensitive attributes like sex, race, and native_country which could skew explanations depending on the sample

### 7. TC-other-info:
- StandardScaler applied for Logistic Regression only, EBM uses raw values