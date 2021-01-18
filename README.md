# School District Analysis

## Project Overview

In this project, I helped Maria, a City School District, analyze data on students' standardized test scores and related information. This analysis will help the school board in making decisions regarding the school budgets and priorities.

However, after receiving the initial analysis results, the school noticed there had been some evidence of academic dishonesty; specifically, reading and math grades for Thomas High School ninth-graders appear to have been altered. To uphold state-testing standards, the school board has asked me to replace the math and reading scores for Thomas High School with NaNs while keeping the rest of the data intact. Once I had replaced the math and reading scores, I repeated the school district analysis that I did in the initial analysis and wrote up a report to describe how these changes affected the overall analysis.


## Resources

- Data Source: schools_complete.csv, students_complete.csv
- Analysis File Name: PyCitySchools_Challenge

## Scholl District Analysis Results

- How is the district summary affected?
    - Overall, the metrics for the district summary were decreased slightly, around 0.2% for each metric. Specifically, the **% Passing Math, % Passing Reading, and % Overall Passing** were decreased by **0.2%, 0.1%, and 0.3%** respectively.

![Original District Summary](Resource/district_summary_og.png)
![New District Summary](Resource/district_summary_new.png)

- How is the school summary affected?
    - The only differences are Thomas High School's **% Passing Math, % Passing Reading, and % Overall Passing**. They were decreased slightly, around **0.3%**. This happened because we manipulated the data to exclude Thomas High School's ninth-grade level from the data set.

![Original School Summary](Resource/school_summary_og.png)
![New School Summary](Resource/school_summary_new.png)


- How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
    - It decreased the **% Passing Math, % Passing Reading, and % Overall Passing** by around **0.3%**.  However, even with this change, Thomas High School is standing at **2nd place** of the top schools that have the **highest % Overall Passing**.

![Top School](Resource/top_schools.png)

- How does replacing the ninth-grade scores affect the following:
    - Math and reading scores by grade: The only difference is at the ninth-grade level, Thomas High School **does not have values** because we already deleted this information in previous steps. Other values still remained the same.

    ![Math score by grade](Resource/thomas_math_score.png)
    ![Reading score by grade](Resource/thomas_reading_score.png)

    - Scores by school spending, Scores by school size, and Scores by school type: These metrics **remained the same** because we only deleted the reading and math scores, not the budget, school size, and school type.

## School District Analysis Summary

There are three major changes to the school district analysis after reading and math scores have been replaced:

- The **% Passing Math, % Passing Reading, and % Overall Passing** were decreased in the district summary.
- The **% Passing Math, % Passing Reading, and % Overall Passing** were decreased in the school summary. However, even with the change, Thomas High School is still standing at **2nd place** of the top schools with the **highest % Overall Passing**.
- There is no value for the Math and Reading scores for the ninth-grade at Thomas High School because we already deleted those values.



