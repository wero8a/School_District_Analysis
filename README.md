# School District Analysis Report

## Overview of the school district analysis:
The purpose of this analysis is to prepare student standardized test data for analysis and presentation in different formats to provide insights about performance, trends, and patterns. This will inform board members and help make strategic decisions at the school and district level. 

## Resources:
- Conda Version 4.14
- Jupyter notebook 6.4.8
- Python 3.7.13
- GitBash version 2.37.1

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
In our original code we can see that about 93% of students passed their math exams and about 97% passed their reading exams at *Thomas High School*. 97% is an absurdly high pass rate if we consider that approximately 1600 students attend "Thomas High School". It is no wonder that the board members noticed there was an irregularity in our data.
#### Original Code School Summary
![image](https://user-images.githubusercontent.com/110706169/189081044-80e387f1-e5f3-4833-a8c3-702aa863555b.png)

![image](https://user-images.githubusercontent.com/110706169/189080479-b215279c-1cb4-4337-892f-050ecd5188b0.png)


#### Challenge Code School Summary
![image](https://user-images.githubusercontent.com/110706169/189081106-abb2636c-10e9-49f7-9916-38aca7932555.png)

![image](https://user-images.githubusercontent.com/110706169/189080118-1c4906ab-4e6d-4ca4-be61-62728cbcd7e2.png)

After nulling grade scores in math and reading for 9th graders at "Thomas High School" we were left with the table shown above. Since we are not counting scores for 9th graders; naturally, these statistics are only considering students in the grades 10th through 12th.

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
![image](https://user-images.githubusercontent.com/110706169/189089450-7ab66c7c-05b4-4b1f-b2ff-690b502bd1c1.png)

In our original code we can see that *Thomas High School* is ranked 2nd among the 14 other schools in the list. 

![image](https://user-images.githubusercontent.com/110706169/189093160-64e29fd2-b671-4cce-a26b-023a6a3d39c6.png)

After removing the grades for 9th graders, *Thomas High School* dropped to rank 8. This could potentially affect the board member's decision to allocate more or less money for the school.

### How does replacing the ninth-grade scores affect the following?
   ####  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Math Scores by Grade &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Reading Scores by Grade
![image](https://user-images.githubusercontent.com/110706169/189098182-b3cb42fb-8318-4c90-b752-965042c019fc.png) ![image](https://user-images.githubusercontent.com/110706169/189099415-bebc1c86-d332-4b8d-ab9f-dfa47eabbe3a.png)

 Replacing the ninth-grade scores for math and reading will show as null in the 9th grade column in the tables above.

 ### Scores by school spending:
 #### Challenge Code
 ![image](https://user-images.githubusercontent.com/110706169/189101204-ffceeb62-8de9-404e-9b96-457e6bc01a44.png) 
 
 #### Original Code
![image](https://user-images.githubusercontent.com/110706169/189102386-76411f8d-3e4f-41ad-9682-96e755eb9cba.png) ![image](https://user-images.githubusercontent.com/110706169/189104578-7a8f1662-2ef2-435f-b3e9-3f0f8ccba9a3.png)

  Replacing the ninth-grade scores has virtually no effect on scores by school spending especially since we are rounding our percentages to the nearest number.
 ### Scores by school size:
 #### Challenge Code
![image](https://user-images.githubusercontent.com/110706169/189106417-ca1b0221-dcaf-4448-9841-9c0ad5665703.png)
 #### Original Code
![image](https://user-images.githubusercontent.com/110706169/189106290-dbc8e736-f489-4025-9c44-4bd7e7b5616f.png)

*Thomas High School* has a total of 1635 students. Even if we remove the 461 9th graders; *Thomas High School* is still a medium size school. The score by school size remains unaffected by removing the ninth graders data.
 ### Scores by school type:
 #### Challenge Code
 ![image](https://user-images.githubusercontent.com/110706169/189107421-32fe1350-87d2-4002-8dc0-f8bef6d6084a.png)

 #### Original Code
 ![image](https://user-images.githubusercontent.com/110706169/189107565-feac5ce5-5916-4698-9c96-3dba1acf6a99.png)

The scores determined by school type remain unaffected even after we remove the *Thomas High School* ninth-grader data.
## Summary:

Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
1. *Thomas High School's* ranking dropped from rank 2 to rank 8 after we removed the ninth-grader data.
2. The *% Overall Passing* dropped from 90.6% to 65.1% for *Thomas High School* .
3. Data for *Thomas High School* ninth-graders will display "NaN" for reading and math when scoring by grades.
4. Overall, the data is not too skewed and can still be used to make a strategic decision on all schools but *Thomas High School*. The anullation of data had a negligible impact for the rest of the schools, but further analysis should be postponed until we get the correct data for *Thomas High School* ninth-graders.
