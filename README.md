# Game-LiveOps-Analysis
**CONTEXT**
1. All users in Russia and using Android devices are playing the game with version 1.5.2.

2. Imagine you are a LiveOps team member and after working on data of game version 1.5.2, you found that the tutorial was not good forthe users experience.
  
3. Hence, you decided you would roll out a new version 1.6.0 to change the Tutorial in-game and you expected this would help increase user experience.

**Special Information:**

The game version 1.6.0 has rolled out 50% since 28-10-2023, meaning 50% of new users will keep playing game version 1.5.2 and 50% of the remaining will play the new version 1.6.0. You started collecting the data from 28-10-2023 to 10-11-2023 to analyze.

**QUESTIONS**

1. How can we know if the improvement of Tutorial in-game version 1.6.0 has impacted the User Experience better than in-game version 1.5.2?
   
2. Can we roll out 100% game version 1.6.0 to all users or not? Why? (Analyze and evaluate the 2 versions).
 
3. Based on the data and your experience with the game, do you have any ideas to improve our User Experience?
### Table of Contents
- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Conclusion](#conclusion)
  
### Prorject Overview
This report analyzes the impact of improvements in the tutorial of game 
version 1.6.0 compared to version 1.5.2. I examine various user metrics 
including Daily Active Users (DAU), retention rates, win rates, and session 
durations. The findings suggest that version 1.6.0 significantly improves user 
experience in several areas, although there are some areas of concern such as 
win rates. Key recommendations include rolling out version 1.6.0 to all users 
and further enhancing the tutorial and balancing game difficulty.

### Data Sources
Internal data so I can't share with you

### Tools
 • Python: Data Cleaning and Analysis

 ### Introduction
 The objective of this analysis is to determine if the changes in game version 
1.6.0, particularly the improved tutorial, have positively impacted the user 
experience compared to version 1.5.2. We use statistical methods to analyze 
user engagement and retention metrics

**1. How can we know if the improvement of Tutorial in-game version 1.6.0 has impacted the User Experience better than in-game version 1.5.2?**

The analysis includes key performance indicators such as tutorial completion rates, daily active users (DAU), session duration and win rates.

**a) Tutorial Completion Rates**
Version 1.5.2: 95.70%
Version 1.6.0: 95.86%
The slight increase in completion rates for version 1.6.0 indicates that the 
improvements made to the tutorial have positively impacted user 
engagement.
Impact of Tutorial Improvements: Tutorial Drop-Off Rates
The lower drop-off rates in version 1.6.0 suggest that users are more engaged 
with the updated tutorial. Potential reasons for this improvement include 
better clarity, interactivity, and pacing of the tutorial steps.
Version 1.5.2: Significant drop-off after step 4.
Version 1.6.0: Remains at 100% until step 8.
![image](https://github.com/Huy24vt/Game-LiveOps-Analyst/assets/130732635/f0669786-feff-490e-b9b2-a53c51b17800)

**b) Retention Rates:**

**Day 1 Retention:**

Z-statistic: -2.485984455187577

P-value: 0.012919360874932801

Interpretation: The p-value is less than 0.05, indicating a significant difference in Day 1 retention rates between versions. Version 1.6.0 has a statistically significant impact on Day 1 retention.

**Day 7 Retention:**

Z-statistic: -4.54730878112399

P-value: 5.433624995471488e-06
Interpretation: The p-value is much less than 0.05, indicating a highly significant difference in Day 7 retention rates between versions. Version 1.6.0 has a statistically significant impact on Day 7 retention.
![image](https://github.com/Huy24vt/Game-LiveOps-Analyst/assets/130732635/607c17ff-6505-4b51-9100-c7a66480cdec)
Both versions show a significant drop from 100% on day 0 to around 30% on day 1. However, version 1.6.0 maintains a slightly higher retention rate after the first day.

**c) Daily Active Users (DAU)**
![image](https://github.com/Huy24vt/Game-LiveOps-Analyst/assets/130732635/6c34ed2a-bf26-4000-8372-02b4c61b50c0)
**Independent T-test Results:**

T-statistic: -0.3756735153114964

P-value: 0.7102073236016677

The p-value is greater than 0.05, indicating no significant difference in DAU between versions 1.5.2 and 1.6.0.

**d) Session Duration**
![image](https://github.com/Huy24vt/Game-LiveOps-Analyst/assets/130732635/6f41eed6-7596-49f3-ae1f-61dcf8b10897)
**Paired T-test Results:**

T-statistic: 29.05

P-value: 8.45e-186

The paired T-test results show a highly significant difference in session duration between game versions 1.5.2 and 1.6.0. The T-statistic of 29.05, 
combined with an extremely low P-value of 8.45e-186, indicates that the mean session duration for version 1.6.0 is substantially greater than for version 1.5.2. 
This significant increase in session duration suggests that players are more engaged with the game in version 1.6.0, spending more time in the game per session. Longer session durations are often associated with better retention rates and higher potential for in-game purchases, contributing positively to the game's revenue.
![image](https://github.com/Huy24vt/Game-LiveOps-Analyst/assets/130732635/1b329b46-a47b-442d-9fe2-a7f323cb4b4c)

**e) Win Rates**

Version 1.5.2: 21.76%

Version 1.6.0: 20.03%

Chi-square Results:

Statistic: 271.35

P-value: 5.78e-61

The win rate for version 1.6.0 is slightly lower than that for version 1.5.2, with a difference of approximately 1.73 percentage points. The Chi-square test results show a highly significant difference between the win rates of the two versions, as indicated by the statistic of 271.35 and an extremely low P-value of 5.78e-61. This suggests that the difference in win rates is not due to random chance but is statistically significant.While the win rate for version 1.6.0 is slightly lower than that of version 1.5.2, the overall positive engagement and retention metrics suggest that the improvements made in version 1.6.0 have enhanced the user experience. It is recommended to continue monitoring and balancing game difficulty to ensure that the game remains engaging and enjoyable for all players.

While the win rate for version 1.6.0 is slightly lower than that of version 1.5.2, the overall positive engagement and retention metrics suggest that the improvements made in version 1.6.0 have enhanced the user experience. It is recommended to continue monitoring and balancing game difficulty to ensure that the game remains engaging and enjoyable for all players.

**2. Can we roll out 100% game version 1.6.0 to all users or not?**
   
Based on the data analysis:

**a) Pros of Version 1.6.0:**

- Significant improvement in Day 1 and Day 7 retention rates, indicating better initial user engagement and sustained usage.

- Longer session durations, suggesting users are more engaged and spend more time in the game.

- Slightly higher tutorial completion rate, showing the new tutorial is effective.

**b) Cons of Version 1.6.0:**

- No significant difference in DAU, suggesting overall daily engagement is similar to version 1.5.2.

- Lower win rate, which could negatively impact user satisfaction and perception of the game's difficulty.

**Conclusion:**

**Should version 1.6.0 be rolled out to all users?**

**Yes**, but with caution. The significant improvements in retention rates and session durations suggest that version 1.6.0 enhances user 
engagement and experience. However, the lower win rate indicates a potential issue with game balance or difficulty, which could affect long-term user satisfaction.

**Recommendation:**

**Monitor and Adjust:** Roll out version 1.6.0 to all users but closely monitor user feedback and game performance metrics. If the lower win 
rate continues to negatively impact user satisfaction, consider making adjustments to the game's difficulty or providing additional support to help users succeed.

**Continuous Improvement:** Keep iterating on the tutorial and other game features to ensure a balanced and enjoyable experience for all users.

**3. Suggestions for Further Improvement**
   
**Enhanced Tutorial Design**

Recommendation: Introduce more interactive elements and rewards for completing each step to maintain engagement beyond step 8. Consider adding checkpoints or progress indicators.

**Balancing Game Difficulty**

Recommendation: Rebalance the difficulty of early game levels to ensure new players do not find the game too challenging. Implement adaptive difficulty that adjusts based on player performance. 
