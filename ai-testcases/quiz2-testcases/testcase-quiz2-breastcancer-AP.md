# AI Testcase
_ // This file has a template for recording testcases for chatbots_

### 1. TC-identifier: 
Alandis-Patterson-BreastCancer01

### 2. TC-name: 
Breast Cancer Classification Explainability Test

### 3. TC-objective: 
Evaluate whether an AI model trained on the Breast Cancer dataset produces
accurate binary cancer classification and provides accurate
graph representation using LIME and Explainable Boost Classifier explanation methods

### 4. TC-input: 
- Breast Cancer dataset (sklearn.datasets.load_breast_cancer())
- Models: Logistic Regression, Random Forest, and EBM
- Explanation method: EBM and LIME

### 5. TC-reference-output: 
- Logistic Regression Accuracy: 0.9825
- Explainable Boost Classifier Breast Cancer Accuracy: 0.9649
- Random Forest Breast Cancer Accuracy: 0.9561
- Top 3 Features: worst texture, worst concave points, and worst perimeter

### 6. TC-harm-risk-info: 
- HC1-incorrect-info: Incorrect classification could lead to a missed cancer diagnosis or unnecessary treatment
- HC3: Breast cancer is said to be more common in different demographics so explanation can be inaccurate

### 7. TC-other-info: 
- StandardScaler applied for only Logistic Regression
