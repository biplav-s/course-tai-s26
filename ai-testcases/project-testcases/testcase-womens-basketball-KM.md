### 1. TC-identifier: 
Kennedy Marren
Womens Basketball TC 02 

### 2. TC-name: 
Similar record matchup with differing strength of schedule

### 3. TC-objective: 
Evaluate whether the model overvalues win-loss record when a team has faced weaker opponents, and whether it is biased toward teams with an easier strength of schedule rather than reflecting team quality.

### 4. TC-input: 
Duke (26-8 record), College of Charleston (27-6 record)

### 5. TC-reference-output: 
Duke wins their recent matchup against College of Charleston, 81-64.

### 6. TC-harm-risk-info: 
This test case poses a risk of favoring teams with easier schedules while failing to account for opponent quality. There is an HC1 (incorrect information) risk, as the model may produce inaccurate predictions due to the lack of a feature representing strength of schedule. There is also an HC3 (unstable extra user info) risk, since a team’s record is often used as an indicator of performance, but in specific matchups where strength of schedule differs significantly, this indicator may become misleading. 

### 7. TC-other-info: 
This test case focuses on evaluating whether the model appropriately incorporates contextual factors such as strength of schedule, rather than relying solely on win-loss record. It is useful for identifying scenarios where teams with inflated records due to weaker opponents or weaker conferences may be incorrectly predicted as the stronger team. There is also still a significant lack of parity between teams in women’s college basketball, where a team may perform well against most opponents but still lose by a large margin to a small number of top-tier programs, therefore it is important to capture this in the data. 