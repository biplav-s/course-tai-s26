### 1. TC-identifier:
Jamius Cheatham  
Breast Cancer TC 01  

### 2. TC-name:
Feature importance in tumor classification  

### 3. TC-objective:
Evaluate whether the model correctly identifies key medical features that influence tumor classification and whether explanation methods highlight meaningful attributes.

### 4. TC-input:
A sample patient with high mean radius, high texture, and high perimeter values  

### 5. TC-reference-output:
Likely malignant tumor classification  

### 6. TC-harm-risk-info:
There is an HC3 (unstable extra user info) risk, as slight variations in medical feature values could lead to different predictions. There is also an HC2 (opinion manipulation) risk if explanation methods misrepresent which features are truly important, potentially misleading medical interpretation.

### 7. TC-other-info:
This test case evaluates whether the model and explanation methods (SHAP and LIME) correctly highlight medically relevant features. It helps verify that the model is not relying on irrelevant or misleading attributes.