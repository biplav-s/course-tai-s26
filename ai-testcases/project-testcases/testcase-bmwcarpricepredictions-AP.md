# AI Testcase
_ // This file has a template for recording testcases for chatbots_

### 1. TC-identifier: 
Alandis-Patterson-BMWCarPredictions01

### 2. TC-name: 
BMW Used Car Price Precition Analysis

### 3. TC-objective: 
Evaluate whether an AI model can properly be trained to study used and new BMW Cars
to predict a price on a used car based on factors like year, transmission, mileage,
and even days on the market

### 4. TC-input: 
- What is the estimated price of a 2014 BMW 328i with 60,000 miles, automatic transmission, AWD, and sedan body type?
- BMW subset

### 5. TC-reference-output: 
- A 2014 BMW 328i with 60,000 miles would be around $10,500
- Price should decrease as mileage increases beyond 60,000 miles

### 6. TC-harm-risk-info: 
- HC1-incorrect-info: Inaccuate price predictions and the AI having a bias or misclassifying older cars and their prices.
- HC3: Dataset reflects a specific time period in the US market predictions so predictions could differ now vs 5 years ago

### 7. TC-other-info: 
- Original dataset was 9 Gigabytes and had to get condensed down and filted to only BMW cars
- a lot of values weren't included because they seemed unnecessary and could cause AI bias
