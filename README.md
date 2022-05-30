# School District Analysis

## Project Overview

Analysis on school district performance, provide insights and visualize the results; using Pandas library, Numpy library, and Jupyter Notebook with Python.<br/>

In this project we will work with Maria, the chief data scientist for a city school district, to provide the initial analysis based on data collected from many schools and students across the school district.
The School Board would like to understand various performance metrics at the district and school level. This analysis will assist the school board and superintendent in making decisions regarding the school budgets and priorities.

## Purpose

While the School Board is pleased with the insights that we have provided, it has been identified that there is some anomalies in the data, in particular in the math and reading scores of the grade 9 students at Thomas High School. 
In order to ensure these results do not skew the analysis, the entire scores of ninth grade class of Thomas High School replaced with NaN. We will now review how this change impacted various parts of the first analysis.

### Resources
:card_file_box: Schools Data : [schools_complete.csv](/Resources/schools_complete.csv)<br/>
:card_file_box: Students Data : [students_complete.csv](/Resources/students_complete.csv)<br/>
:card_file_box: Anaconda Software : [64-Bit Graphical Installer](https://www.anaconda.com/products/distribution)<br/>



## Analysis Results
Using bulleted lists and images of DataFrames as support, address the following questions:
- How is the district summary affected?
- How is the school summary affected?
- How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
- How does replacing the ninth-grade scores affect the following:
    - Math and reading scores by grade
    - Scores by school spending
    - Scores by school size
    - Scores by school type
    <br/>
    
    
### Impact on District Analysis

 ***District Summary - Original***
 ![ds-01.png](/images/ds-01.png)
 <br/><br/>
 ***District Summary - Updated***
 ![ds-02.png](/images/ds-02.png) 
 <br/>
The change of adding NaN value to all grade 9 of Thomas High School math and reading scores, did not have a large impact on the district summary analysis. It's important to consider there are only 461 students in grade 9 at Thomas High School, and the total student count is 39,170, which is 1.2% of the total student, so removing their math and reading scores can only impact the averages so much. <br/>

### Impact on school summary
***Top Schools - Original***
![ps-01.png](/images/ps-01.png)
<br/><br/>
***Top Schools - Updated***
![ps-02.png](/images/ps-02.png)

- The ranking of the top schools including Thomas High School, was not affected by the update.
- While the average math, reading and overall scores at Thomas High School were impacted with the update, the changes were not enough to change its relative ranking in compare with other schools.

***Bottom Schools - Original***
![bs-01.png](/images/bs-01.png)

***Bottom Schools - Updated***
![bs-02.png](/images/bs-02.png)
<br/>
The ranking of the bottom schools was not affected by the update, as the metrics  only impacted at Thomas High School.

### Impact on Math and Reading Scores by Grade
***- Math Scores***

<table>
  <tr>
    <th>- Original -</th>
    <th>- Updated -</th>
  </tr>
  <tr>
    <td><img src="images/ms-01.png"></td>
    <td><img src="images/ms-02.png"></td>
  </tr>
</table>

<br/>


***- Reading Scores***

<table>
  <tr>
    <th>- Original -</th>
    <th>- Updated -</th>
  </tr>
  <tr>
    <td><img src="images/rs-01.png"></td>
    <td><img src="images/rs-02.png"></td>
  </tr>
</table>
<br/>

The only score that is impacted on this DataFrame is that the grade 9 students at Thomas High School have Nan instead of a grade for both math and reading. If we ran a sum or mean of the DataFrame, we would see a difference between the orignal and updated.

### Impact on Scores by School Spending
***Original***
***Updated***

### Effects on Scores by School Size
***Original***
***Updated***


### Impact on Scores by School Type
***Original***
***Updated***


## Summary
Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
- District Analysis - changes to all scores by less than 0.5 percentage points (or change by less than 0.5%) - no impact to school or student count.
- Top School Ranking - no change to ranking, however Thomas High School scores did change, but by less than 1 percentage point (or changed by less than 1%) for each metric.
- Scores by School Size - changes to Medium (1000-2000) grouping for all scores by less than 0.1 percentage points (or change by less than 0.1%).
- Scores by School Type - chages to Charter type grouping for all scores by less than 0.1 percentage points (or change by less than 0.1%).

<br/>
