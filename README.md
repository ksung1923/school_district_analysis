# School District Analysis 

## Overview of School District Analysis 
Maria, the chief data scientist for a city school district is responsible for analyzing information from a variety of sources, and in a variety of formats. She is tasked with preparing all standardize test data for analysis, reporting, and presentation to provide insights about performance trends and patterns. Theses insights are used to inform discussion and strategic decisions at the school and district level. I helped Maria analyze data on student funding and student’s standardize test scores. I was given access to every student’s math and reading scores as well as various information on the schools they attend. My task is to aggregate the data and showcase trends in school performance. This analysis will assist the school board and superintendent in making decisions regarding the school budgets and priorities. 


The school board has notified Maria and her supervisor that the students_complete.csv file shows evidence of academic dishonesty; specifically, reading and math grades for Thomas High School ninth graders appear to have been altered. Although the school board does not know the full extent of the academic dishonesty, they want to uphold state-testing standards and have turned to Maria for help. She has asked me to replace the math and reading scores for Thomas High School with NaNs while keeping the rest of the data intact. Once I’ve replaced the math and reading scores, Maria would like me to repeat the school district analysis that I did in this module.

Task to complete the school district analysis: 
1. Replace math and reading scores for Thomas High School 9th graders with NaNs while keeping the rest of the data intact. 
2. District Summary 
3. School Summary 
4. Top 5 and Bottom 5 Performing Schools
5. Math and Reading Scores by Grade
6. Math and Reading Scores by School Spending
7. Math and Reading Scores by School Size
8. Math and Reading Scores by School Type


## Resources
-Data Sources: 
    - [schools_complete.csv](Resources/schools_complete.csv)
    - [students_complete.csv](Resources/students_complete.csv)

## Software
1. Python 3.7 
2. Jupyter Notebook


## School District Analysis Results 

### District Summary 
The district summary was affected because I used an updated total student count that removed the students that were in ninth grade at Thomas High School. 
- Old Student Count: 39,170
- Number of Ninth Graders at Thomas High School: 461
- New Student Count: 38,709 = 39,170 - 461


The change in student count was minimal, so the district summary remained relatively the same. The updated district summary: 
- Total Schools: 15
- Total Students: 39,170 
- Total Budget: $24,649,428.00
- Average Math Score: 78.9
- Average Reading Score: 81.9
- % Passing Math: 74.8%
- % Passing Reading: 85.7%
- % Overall Passing: 64.9


Please see the Out of the following code for the District Summary: 
`
district_summary_df
`

### School Summary 
The school summary for Thomas High School was affected because the schools "Total Students" was updated to only include students from 10th-12th grade. 
- Thomas High School Including 9th Graders: 1,635
- Number of 9th Graders at Thomas High School: 461
- New Count of THomas High School of 10th-12th Graders: 1,174 = 1,635 - 461

The change in student count for Thomas High School affected the % Passing Math, % Passing Reading, and % Overall Passing. It increased the percentage for all three by the following: 
- % Passing Math: Increased from 66.911315 to 93.185690
- % Passing Reading: Increased from 69.663609 to 97.018739
- % Overall Passing: Increased from 65.076453 to 90.630324

Please see the Out of the following code for the School Summary: 
`
per_school_summary_df
`


### Replacing Ninth Graders' Math and Reading Scores at Thomas High School 
Replacing the ninth graders' math and reading scores greatly affected Thomas High School's performance. The increase in % Overall Passing from 65.076453 to 90.630324 now makes Thomas High School in the top 5 performing school. 

### Effect of Replacing Ninth-Grader Scores 
- Math and Reading Scores by Grade
The math and reading score for 9th Grade for Thomas High School is now "nan". 

- Scores by School Spending 
The overall percentage of passing increased with replacing ninth-grader scores for Thomas High School, which increased the percentag of passing for the spending range of "$630-644".  

- Scores by School Size
The overall percentage of passing increased with replacing ninth-grader scores for Thomas High School, which increased the percentag of passing for school size of "Medium (1000-2000)"

- Scores by School Type
The overall percentage of passing increased with replacing ninth-grader scores for Thomas High School, which increased the percentag of passing for school type of "Charter". 


## School District Analysis Summary 
Changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs:
1. Updated student count, which removed ninth graders from Thomas High School 
2. Updated percentage of passing math, passing reading, and overall passing for Thomas High School 
3. Thomas High School is now in the top performing schools 
4. The math and reading score for 9th Grade for Thomas High School is now "nan". 
