# School_District_Analysis

## Overview
Maria, a chief data scientist for a school district, is responsible for analysing information. In this task, she needs to analyse test data in order to help understand performance trends and patterns. Such study will help the school board and the superintendent in budgeting and priorities. 
* The main task is to agregate data (respecting Ferpa - Family Educational Rights and Privacy Act) providing various views on performance taking into account parameters like school type, size, budget per student, etc.
* A second task is to analyse the impact on numbers if a given subset of data is removed from the analysis. It was reported that the scores of Thomas High School 9th grade were not reliable, that there had been some sort of disonesty when reporting data. The idea is to remove this data from the analysis and understand how this removal impacted on the numbers.

## Results
Several approaches were used to analyse data - from more generic to more specific ones. The results are listed below - comparing the discrepancies that aroused from the removal of part of the data. The number of records excluded from our analysis was 461, representing 1.17% of the total.

### District Summary
In the District Summary, the idea is to have an overview of all schools in one single line. It shows the total number of students, total budget and average scores. The first picture shows the table with all data and the second without Thomas High School 9th graders. It is easy to notice that the change is minimal  when we remove the "suspect" data.
![district_summary_complete](/resources/district_summary_complete.png)

![district_summary_without_Thomas9th](/resources/district_summary_without_Thomas9th.png)

### School Summary
In the School Summary, no relevant change was noticed either. The average and percentage of passing scores were pretty much the same after the correct adjustments to reflect only students from 10th to 12th grades. The first extract shows the complete data and the second one shows the partial version. It is important to state that, even though the second one shows 1635 students, averages and percentages were calculated based on 1174 students - corresponding to 10th to 12th grade. We chose to leave 1635 as the total number of students because this is the real number of students at Thomas High School and such number is used for other purposes such as *per student budget*.

![school_summary_complete](/resources/school_summary_complete.png)

![school_summary_without_Thomas9th](/resources/school_summary_without_Thomas9th.png)

### Top Performing Schools
Once again we notice that the change was so small that it can be considered irrelevant. When considering all data, Thomas High School placed second as the top performing school and the same happens when 9th graders' data is removed.

![top_5_complete](/resources/top_5_complete.png)

![top_5_without_Thomas9th](/resources/top_5_without_Thomas9th.png)

### Bottom Performing Schools
Given the only data that changed was from Thomas High and it is not among the bottom performing schools, the bottom performing list is kept before and after the removal of data.

![bottom_5_complete](/resources/bottom_5_complete.png)

![bottom_5_without_Thomas9th](/resources/bottom_5_without_Thomas9th.png)

### Average Math Score for each grade level from each school

![Math_Scores_complete](/resources/Math_Scores_complete.png)

![Math_Scores_without_Thomas9th](/resources/Math_Scores_without_Thomas9th.png)


### Average Reading Score for each grade level from each school

![Reading_Scores_complete](/resources/Reading_Scores_complete.png)

![Reading_Scores_without_Thomas9th](/resources/Reading_Scores_without_Thomas9th.png)

### Scores by School Spending per Student

![Spending_Ranges_complete](/resources/Spending_Ranges_complete.png)
![Spending_Ranges_without_Thomas9th](/resources/Spending_Ranges_without_Thomas9th.png)


### Scores by School Size

![School_size_complete](/resources/School_size_complete.png)
![School_size_without_Thomas9th](/resources/School_size_without_Thomas9th.png)


### Scores by School Type

![School_type_complete](/resources/School_type_complete.png)
![School_type_without_Thomas9th](/resources/School_type_without_Thomas9th.png)


## Summary
