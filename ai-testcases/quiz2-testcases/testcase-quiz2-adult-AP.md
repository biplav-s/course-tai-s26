# AI Testcase
_ // This file has a template for recording testcases for chatbots_

### 1. TC-identifier: 
Alandis-Patterson-Adult01

### 2. TC-name: 
Adult Income Classification Explainability Test

### 3. TC-objective: 
Evaluate whether an AI model trained on the Adult Income dataset produces
accurate binary income classification and provides accurate
graph representation using LIME and Explainable Boost Classifier explanation methods

### 4. TC-input: 
- Adult dataset(https://archive.ics.uci.edu/ml/machine-learning-databases/adult/adult.data)
- Models: Logistic Regression, Random Forest, and EBM
- Explanation method: EBM and LIME

### 5. TC-reference-output: 
- Logistic Regression Accuracy:  0.8279
- Explainable Boost Classifier Adult Income Accuracy:  0.8724
- Random Forest for Adult Income Accuracy: 0.8604
- Top 3 Features: Age, Marital Status, and Captial Gain



### 6. TC-harm-risk-info: 
- HC1-incorrect-info: The incorrect amount of income can lead to AI bias which could then affect outcomes of banking loans
- HC3: LIME explanations may have trouble with different population samples

### 7. TC-other-info: 
- some data is not scaled
- some data features make a minimum difference
