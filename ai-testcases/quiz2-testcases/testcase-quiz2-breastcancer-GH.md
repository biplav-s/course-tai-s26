# AI Testcase

### 1. TC-identifier:
Hulbert-Gage-Breast-Cancer

### 2. TC-name:
Breast Cancer Classification Explainability Test

### 3. TC-objective:
Determine if an AI model trained with the Breast Cancer dataset can accurately classify tumors as malignant or benign, and whether SHAP and LIME produce consistent and meaningful explanations for the predictions.

### 4. TC-input:
- Breast Cancer Wisconsin dataset (sklearn.datasets.load_breast_cancer)
- Models: Logistic Regression (whitebox), Gradient Boosting (blackbox)
- Explanation methods: SHAP (LinearExplainer and TreeExplainer), LIME (local explanations)

### 5. TC-reference-output:
- Logistic Regression Accuracy: ~0.96
- Gradient Boosting Accuracy: ~0.97
- Top features identified by SHAP: worst concave points, worst perimeter, mean concave points
- SHAP and LIME agree on top contributing features for individual predictions
- High values of worst concave points push predictions toward malignant

### 6. TC-harm-risk-info:
- HC1-incorrect-info: A false benign prediction for a malignant tumor could delay treatment and cause serious patient harm
- HC4-incomprehensible-ai: If SHAP and LIME disagree on top features, the model explanation is unreliable and should not be trusted in a clinical setting

### 7. TC-other-info:
- No sensitive demographic attributes in this dataset so bias risk is lower than Adult Income
- StandardScaler applied for Logistic Regression; Gradient Boosting uses raw values