# Quiz 2 AI Testcase: Survey Data Project


### 1. TC-identifier: 
Alex Ervin TC-SD01

### 2. TC-name: 
Logical Inconsistencies

### 3. TC-objective: 
To see if the detection model is capable of detecting logical inconsistencies across inputted responses.   

### 4. TC-input: 
Q3. How many children do you have? -> Answer: 3
...
Q6. How many children below the age of 10? -> 2
Q7. How many children at or above the age of 10? -> 0
### 5. TC-reference-output: 
The model should add weight to the decision being more likely AI generated or automated due to the inconsistencies. Human respondants are likely to have a mistake every once in a while, but repeated mistakes such as this in conjunction with other indicators could results in a prediction of  "Automated/AI Generated".

### 6. TC-harm-risk-info: 
HC3-unstable: The AI answerer would need to keep track of its state and be aware of various constraints set by previous answers. 

### 7. TC-other-info: 


----

This file is associated with the book, Building Trustworthy Chatbots: A Risk-aware Approach with Use Cases, by Biplav Srivastava, 2025