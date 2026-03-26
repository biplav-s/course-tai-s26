# AI Testcase (TC) Template
_ // This file has a template for recording testcases for chatbots_

### 1. TC-identifier: 
test-case-smartphone-battery-health
### 2. TC-name: 
High Usage and Temperature Battery Degradation Test
### 3. TC-objective: 
Evaluate wheter the AI model correctly predicts lower battery health under high temperature and heavy use conditions
### 4. TC-input: 
device age = 22 months, battery_capacity = 3000mAh, Screen time = 7.6 hours/day, charging cycles = 11.5/week, temperature = 37.4 celsius, usage = high

### 5. TC-reference-output: 
battery health should be low indicating significant battery degradation

### 6. TC-harm-risk-info: 
HC1-incorrect-info: Incorrect predictions could mislead users about battery health
Model may behave inconsistently across different usage patterns or devices


### 7. TC-other-info: 
Continuous testing is needed to improve reliability and fairness

----

This file is associated with the book, Building Trustworthy Chatbots: A Risk-aware Approach with Use Cases, by Biplav Srivastava, 2025
