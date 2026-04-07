### 1. TC-identifier:
Jamius Cheatham  
Adult Income TC 01  

### 2. TC-name:
Impact of work and education features on income classification  

### 3. TC-objective:
Evaluate whether the model appropriately considers key socioeconomic features such as education level and hours worked when predicting income level.

### 4. TC-input:
An individual with a high level of education, stable occupation, and long working hours  

### 5. TC-reference-output:
Likely income greater than 50K  

### 6. TC-harm-risk-info:
There is an HC2 (opinion manipulation) risk if the model reinforces biased assumptions about income based on certain features such as occupation or education. There is also an HC3 (unstable extra user info) risk because preprocessing and encoding of categorical variables may lead to inconsistent interpretations across similar individuals.

### 7. TC-other-info:
This test case evaluates whether explanation methods correctly identify the most influential features in income prediction. It also helps verify that preprocessing does not distort feature importance.