# AI Testcase (TC) For Telco Churn Data

### 1. TC-identifier: 
TC-TC-01

### 2. TC-name: 
Extremely Long Tenure, Zero Service Usage

### 3. TC-objective: 
Evaluate model behavior for when a loyal customer hasn't actually used any services.

### 4. TC-input: 
tenure: 200
PhoneService: No
InternetService: No
...

### 5. TC-reference-output: 
Predict low-churn due to long tenure, but with extreme uncertainty since customer uses no servies.

### 6. TC-harm-risk-info: 
HC1 - incorrect info
HC5 - contradictory input
The AI model may predict the customer is unlikely to churn due to the high tenure; however, if they aren't using any services, the customer may actually be unsatisfied. In other words, the model may wrongly predict the outcome. The model may not know what to do with contradictory output. Which way should it predict?

### 7. TC-other-info: 
Useful for checking whether some features are overweighted.

----

This file is associated with the book, Building Trustworthy Chatbots: A Risk-aware Approach with Use Cases, by Biplav Srivastava, 2025
