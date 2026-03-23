# AI Testcase

### 1. TC-identifier:
Gage-Hulbert-Watch-Price

### 2. TC-name:
Luxury Watch Price Prediction Test

### 3. TC-objective:
Determine if AI model trained with the Luxury Watch Listings dataset can accurately predict the price of a watch given its characteristics (brand, model, material, movement type, etc.) and provide meaningful explanations for what drives price predictions.

### 4. TC-input:
- Luxury Watch Listings dataset (Kaggle - Luxury Watch Listings)
- Models: Logistic Regression, Linear Regression, Random Forest
- Explanation methods: SHAP (global + local), LIME (local)
- Sample input: Brand = Rolex, Model = Submariner, Case Material = Stainless Steel, Diameter = 41mm, Condition = New

### 5. TC-reference-output:
- Model predicts a price range consistent with known Rolex Submariner market value (~$10,000-$14,000)
- Top features identified by SHAP: Brand, Model, Case Material, Condition
- SHAP and LIME agree on top 3 features driving the prediction
- Higher-end brands (Patek Philippe, Audemars Piguet) consistently predict higher prices than mid-tier brands

### 6. TC-harm-risk-info:
- HC1-incorrect-info: An inaccurate price prediction could mislead buyers or sellers in real transactions, resulting in financial loss
- HC3-unstable-extrauserinfo: Watch listings may have inconsistent or missing data (such as missing dial color, strap material) which could make predictions unstable across different samples

### 7. TC-other-info:
- Price column may need log transformation due to high variance across luxury tiers
- Some brands may have very few listings, making predictions for rare brands less reliable