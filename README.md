# School District Analysis

## Project Overview

Analysis on school district performance, provide insights and visualize the results using <b>Numpy</b>.<br/>
In this project we will provide the initial analysis based on data collected from many schools and students across the school district.
The School Board would like to understand various performance metrics at the district and school level. This analysis will assist the school board and superintendent in making decisions regarding the school budgets and priorities.

## Purpose
After a school board found evidence of academic dishonesty among the grades of one of the district schools, a chief data scientist for the city school district has given us the following tasks to complete the school district data analysis.

1. Replace the math and reading scores for Thomas High School with NaNs while keeping the rest of the data intact.
2. Repeat the school district analysis and recreate the following metrics:
    - The district summary
    - The school summary
    - The top 5 and bottom 5 performing schools, based on the overall passing rate
    - The average math score for each grade level from each school
    - The average reading score for each grade level from each school
    - The scores by school spending per student, by school size, and by school type
3. Describe how these changes affect the overall analysis.

### Resources
- Schools Data:&nbsp; [schools_complete.csv](/Resources/schools_complete.csv)<br/>
- Students Data:&nbsp; [students_complete.csv](/Resources/students_complete.csv)<br/>
- Anaconda:&nbsp; [Anaconda 64-Bit Graphical Installer](https://www.anaconda.com/products/distribution)<br/>

<br/>

## Analysis Results 
<br/>

### Impact on District Analysis

 ***District Summary - Original***
 ![ds-01.png](/images/ds-01.png)
 <br/><br/>
 ***District Summary - Updated***
 ![ds-02.png](/images/ds-02.png) 
 <br/>
The change of adding NaN value to all grade 9 of Thomas High School math and reading scores, did not have a large impact on the district summary analysis. It's important to consider there are only 461 students in grade 9 at Thomas High School, and the total student count is 39,170, which is 1.2% of the total student, so removing their math and reading scores can only impact the averages. <br/>
<br/>


### Impact on school summary

***Top Schools - Original***
![ps-01.png](/images/ps-01.png)
<br/><br/>
***Top Schools - Updated***
![ps-02.png](/images/ps-02.png)

- The ranking of the top schools including Thomas High School, was not affected by the update.
- While the average math, reading and overall scores at Thomas High School were impacted with the update, the changes were not enough to change its relative ranking in compare with other schools.
<br/>

***Bottom Schools - Original***
![bs-01.png](/images/bs-01.png)

***Bottom Schools - Updated***
![bs-02.png](/images/bs-02.png)
<br/>
The ranking of the bottom schools was not affected after adding NaN value to all grade 9 of Thomas High School math and reading scores.
<br/>
<br/>

### Impact on Math and Reading Scores by Grade

***Math Scores***

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

***Reading Scores***

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

The only score that was impacted on this DataFrame was the grade 9 students at Thomas High School that have NaN instead of a grade for both math and reading.
<br/>
<br/>

### Impact on Scores by School Spending

***Original***

![sps-01.png](/images/sps-01.png)

***Updated***

![sps-02.png](/images/sps-02.png)
<br/>

There was a slight change in this score for the $630-644 group, where Thomas High School is grouped, however the change is small with each metric changing.
<br/>
<br/>


### Effects on Scores by School Size

***Original***

![ss-01.png](/images/ss-01.png)
<br/>

***Updated***

![ss-02.png](/images/ss-02.png)
<br/>
The scores for the Medium size schools changed slightly which Thomas High School included in this group as it has 1,635 students who attend, including the grade 9 students.
<br/>
<br/>

### Impact on Scores by School Type

***Original***
![st-01.png](/images/st-01.png)

***Updated***
![st-02.png](/images/st-02.png)

<br/>
Thomas High School is a Charter type school, so this is why we see changes to the scores for Charter, but no changes to District type school scores and no other school scores were affected.

## Summary
The updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.

- District Analysis : The district as a whole has also had its average math and reading scores decrease, as well as the passing percentages for students.
- Top School Ranking : No change to ranking, however Thomas High School scores did change in the passing rate and average grades.
- Scores by School Size : Changes to Medium (1000-2000) grouping for all scores by less than 0.1 percentage points.
- Scores by School Type : chages to Charter type group for all scores by less than 0.1 percentage points.
 

<br/>
