# School District Analysis Report

## Overview of the school district analysis:
The purpose of this analysis is to prepare student standardized test data for analysis and presentation in different formats to provide insights about performance, trends, and patterns. This will inform board members and help make strategic decisions at the school and district level. 

## Results:
### How is the district summary affected?
The following table shows the results of our analysis for the district using our original code.
#### Original Code District Summary
![image](https://user-images.githubusercontent.com/110706169/189073645-4cd7fb5a-9aca-40bf-b4d0-2f795d4e9124.png)

After being notified by concerned board members that the grades for reading and math in the *9th* grade  at *Thomas High School* have been tampered with. We were asked to null all results for reading and math for that respective class grade.

#### Challenge Code District Summary
![image](https://user-images.githubusercontent.com/110706169/189073441-65421228-1093-41a5-8666-410ce1fdc789.png)

A total of 461 *9th* graders had their test results voided as show on the table above. The new value for **Total Students** changed from 39,170 to 38,709

### How is the school summary affected?
In our original code we can see that about 93% of students passed their math exams and about 97% passed their reading exams at *Thomas High School*. 97% is an absurdly high pass rate if we consider that thousands of students attend "Thomas High School". It is no wonder that the board members noticed there was an irregularity in our data.
#### Original Code School Summary
![image](https://user-images.githubusercontent.com/110706169/189081044-80e387f1-e5f3-4833-a8c3-702aa863555b.png)

![image](https://user-images.githubusercontent.com/110706169/189080479-b215279c-1cb4-4337-892f-050ecd5188b0.png)


#### Challenge Code School Summary
![image](https://user-images.githubusercontent.com/110706169/189081106-abb2636c-10e9-49f7-9916-38aca7932555.png)

![image](https://user-images.githubusercontent.com/110706169/189080118-1c4906ab-4e6d-4ca4-be61-62728cbcd7e2.png)

After nulling grade scores in math and reading for 9th graders at "Thomas High School" we were left with the table shown above. Since we are not counting scores for 9th graders; naturally, these statistics are only considering students in the grades 10th thru 12th.

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
Removing this large chunck of data drastically skews the *% Passed* for reading, math and overall, but atleast it is accurately representing the the *% Passed* for students in the 10th to 12th grade.

- How does replacing the ninth-grade scores affect the following?
   - Math and reading scores by grade
   - Scores by school spending
   - Scores by school size
   - Scores by school type
## Summary:

Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
