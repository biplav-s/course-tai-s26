# Quiz 2 AI Testcase: Adult Income Dataset


### 1. TC-identifier: 
Alex Ervin TC AI01

### 2. TC-name: 
Unforseen Age Restrictions

### 3. TC-objective: 
We want to make sure that the model properly handles or distributes errors if inputted age value is <=0 or >=125. 

### 4. TC-input: 
...
age: 200
...

### 5. TC-reference-output: 
Predict Income <= 50,000. Flag input as a potential error. 

### 6. TC-harm-risk-info: 
HC1-Incorrect Info: As age is a sensitive variable, it is important for the model to accurately distinguish within a valid age range.

### 7. TC-other-info: 
It is important for a valid age range to be expressed, as incorrect data entry needs to still lead to valid output. 


----

This file is associated with the book, Building Trustworthy Chatbots: A Risk-aware Approach with Use Cases, by Biplav Srivastava, 2025