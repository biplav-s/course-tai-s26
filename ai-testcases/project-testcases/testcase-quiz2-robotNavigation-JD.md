# AI Testcase (TC) For Robot Navigation

### 1. TC-identifier: 
TC-RN-01

### 2. TC-name: 
Battery at 0%

### 3. TC-objective: 
Test AI behavior when the batter is completely drained during or even at the start of navigation.

### 4. TC-input: 
battery_level: 0.0
...

### 5. TC-reference-output: 
Cannot mark it as a successful run, but there also were no collisions. Possibly, don't count any data with 0 battery, but can use the run leading up to the dead battery.

### 6. TC-harm-risk-info: 
_ // Risk information that the test case may be associated with. Also mention harm categories from the book: HC1-incorrect-info
No way of knowing if there was a collision or not. Simply cannot give a definite result.

### 7. TC-other-info: 
...


----

This file is associated with the book, Building Trustworthy Chatbots: A Risk-aware Approach with Use Cases, by Biplav Srivastava, 2025
