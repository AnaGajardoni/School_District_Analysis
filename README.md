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

***Complete School Summary***

|           School Type | Total Students | Total School Budget | Per Student Budget | Average Math Score | Average Reading Score | % Passing Math | % Passing Reading | % Overall Passing | Spending Ranges (Per Student) | School Size |                    |
|----------------------:|---------------:|--------------------:|-------------------:|-------------------:|----------------------:|---------------:|------------------:|------------------:|------------------------------:|------------:|--------------------|
|    Bailey High School |       District |                4976 |      $3,124,928.00 |            $628.00 |             77.048432 |      81.033963 |         66.680064 |         81.933280 |                     54.642283 |    $630-644 |  Large (2000-5000) |
|   Cabrera High School |        Charter |                1858 |      $1,081,356.00 |            $582.00 |             83.061895 |      83.975780 |         94.133477 |         97.039828 |                     91.334769 |       <$584 | Medium (1000-2000) |
|  Figueroa High School |       District |                2949 |      $1,884,411.00 |            $639.00 |             76.711767 |      81.158020 |         65.988471 |         80.739234 |                     53.204476 |    $630-644 |  Large (2000-5000) |
|      Ford High School |       District |                2739 |      $1,763,916.00 |            $644.00 |             77.102592 |      80.746258 |         68.309602 |         79.299014 |                     54.289887 |    $630-644 |  Large (2000-5000) |
|   Griffin High School |        Charter |                1468 |        $917,500.00 |            $625.00 |             83.351499 |      83.816757 |         93.392371 |         97.138965 |                     90.599455 |    $630-644 | Medium (1000-2000) |
| Hernandez High School |       District |                4635 |      $3,022,020.00 |            $652.00 |             77.289752 |      80.934412 |         66.752967 |         80.862999 |                     53.527508 |    $645-675 |  Large (2000-5000) |
|    Holden High School |        Charter |                 427 |        $248,087.00 |            $581.00 |             83.803279 |      83.814988 |         92.505855 |         96.252927 |                     89.227166 |       <$584 |      Small (<1000) |
|     Huang High School |       District |                2917 |      $1,910,635.00 |            $655.00 |             76.629414 |      81.182722 |         65.683922 |         81.316421 |                     53.513884 |    $645-675 |  Large (2000-5000) |
|   Johnson High School |       District |                4761 |      $3,094,650.00 |            $650.00 |             77.072464 |      80.966394 |         66.057551 |         81.222432 |                     53.539172 |    $645-675 |  Large (2000-5000) |
|      Pena High School |        Charter |                 962 |        $585,858.00 |            $609.00 |             83.839917 |      84.044699 |         94.594595 |         95.945946 |                     90.540541 |    $585-629 |      Small (<1000) |
| Rodriguez High School |       District |                3999 |      $2,547,363.00 |            $637.00 |             76.842711 |      80.744686 |         66.366592 |         80.220055 |                     52.988247 |    $630-644 |  Large (2000-5000) |
|   Shelton High School |        Charter |                1761 |      $1,056,600.00 |            $600.00 |             83.359455 |      83.725724 |         93.867121 |         95.854628 |                     89.892107 |    $585-629 | Medium (1000-2000) |
|    Thomas High School |        Charter |                1635 |      $1,043,130.00 |            $638.00 |             83.350937 |      83.896082 |         93.185690 |         97.018739 |                     90.630324 |    $630-644 | Medium (1000-2000) |
|    Wilson High School |        Charter |                2283 |      $1,319,574.00 |            $578.00 |             83.274201 |      83.989488 |         93.867718 |         96.539641 |                     90.582567 |       <$584 |  Large (2000-5000) |
|    Wright High School |        Charter |                1800 |      $1,049,400.00 |            $583.00 |             83.682222 |      83.955000 |         93.333333 |         96.611111 |                     90.333333 |       <$584 | Medium (1000-2000) |

### Top Performing Schools
Once again we notice that the change was so small that it can be considered irrelevant. When considering all data, Thomas High School placed second as the top performing school and the same happens when 9th graders' data is removed.

![top_5_complete](/resources/top_5_complete.png)

![top_5_without_Thomas9th](/resources/top_5_without_Thomas9th.png)

### Bottom Performing Schools
Given the only data that changed was from Thomas High and it is not among the bottom performing schools, the bottom performing list is kept before and after the removal of data.

![bottom_5_complete](/resources/bottom_5_complete.png)

![bottom_5_without_Thomas9th](/resources/bottom_5_without_Thomas9th.png)

### Average Math Score for each grade level from each school
The average Math Score shows NaN for Thomas High School 9th graders. Since this was the only portion of data that was touched, all the rest remains the same.

![Math_Scores_complete](/resources/Math_Scores_complete.png)

![Math_Scores_without_Thomas9th](/resources/Math_Scores_without_Thomas9th.png)

***Complete Math Score for each grade level from each school***

|                       |  9th | 10th | 11th | 12th |
|----------------------:|-----:|-----:|-----:|-----:|
|    Bailey High School | 77.1 | 77.0 | 77.5 | 76.5 |
|   Cabrera High School | 83.1 | 83.2 | 82.8 | 83.3 |
|  Figueroa High School | 76.4 | 76.5 | 76.9 | 77.2 |
|      Ford High School | 77.4 | 77.7 | 76.9 | 76.2 |
|   Griffin High School | 82.0 | 84.2 | 83.8 | 83.4 |
| Hernandez High School | 77.4 | 77.3 | 77.1 | 77.2 |
|    Holden High School | 83.8 | 83.4 | 85.0 | 82.9 |
|     Huang High School | 77.0 | 75.9 | 76.4 | 77.2 |
|   Johnson High School | 77.2 | 76.7 | 77.5 | 76.9 |
|      Pena High School | 83.6 | 83.4 | 84.3 | 84.1 |
| Rodriguez High School | 76.9 | 76.6 | 76.4 | 77.7 |
|   Shelton High School | 83.4 | 82.9 | 83.4 | 83.8 |
|    Thomas High School |  nan | 83.1 | 83.5 | 83.5 |
|    Wilson High School | 83.1 | 83.7 | 83.2 | 83.0 |
|    Wright High School | 83.3 | 84.0 | 83.8 | 83.6 |

### Average Reading Score for each grade level from each school
The average Reading Score shows NaN for Thomas High School 9th graders. Once again, this was the only portion of data that was affected, all the rest stays the same.

![Reading_Scores_complete](/resources/Reading_Scores_complete.png)

![Reading_Scores_without_Thomas9th](/resources/Reading_Scores_without_Thomas9th.png)

***Complete Reading Score for each grade level from each school***

|                       | 9th  | 10th | 11th | 12th |
|----------------------:|-----:|-----:|-----:|------|
|    Bailey High School | 81.3 | 80.9 | 80.9 | 80.9 |
|   Cabrera High School | 83.7 | 84.3 | 83.8 | 84.3 |
|  Figueroa High School | 81.2 | 81.4 | 80.6 | 81.4 |
|      Ford High School | 80.6 | 81.3 | 80.4 | 80.7 |
|   Griffin High School | 83.4 | 83.7 | 84.3 | 84.0 |
| Hernandez High School | 80.9 | 80.7 | 81.4 | 80.9 |
|    Holden High School | 83.7 | 83.3 | 83.8 | 84.7 |
|     Huang High School | 81.3 | 81.5 | 81.4 | 80.3 |
|   Johnson High School | 81.3 | 80.8 | 80.6 | 81.2 |
|      Pena High School | 83.8 | 83.6 | 84.3 | 84.6 |
| Rodriguez High School | 81.0 | 80.6 | 80.9 | 80.4 |
|   Shelton High School | 84.1 | 83.4 | 84.4 | 82.8 |
|    Thomas High School |  nan | 84.3 | 83.6 | 83.8 |
|    Wilson High School | 83.9 | 84.0 | 83.8 | 84.3 |
|    Wright High School | 83.8 | 83.8 | 84.2 | 84.1 |

### Scores by School Spending per Student
The elimination of Thomas High School 9th graders scores did not change the scores by school spending per student significantly. The range $630-$644 had minor changes.

![Spending_Ranges_complete](/resources/Spending_Ranges_complete.png)

![Spending_Ranges_without_Thomas9th](/resources/Spending_Ranges_without_Thomas9th.png)


### Scores by School Size
The elimination of Thomas High School 9th graders scores did not change the scores by school size significantly. The medium school range remained the same.

![School_size_complete](/resources/School_size_complete.png)
![School_size_without_Thomas9th](/resources/School_size_without_Thomas9th.png)


### Scores by School Type
The elimination of Thomas High School 9th graders scores did not change the scores by school type significantly. Charter schools continue to outperform the district ones in both scenarios.

![School_type_complete](/resources/School_type_complete.png)
![School_type_without_Thomas9th](/resources/School_type_without_Thomas9th.png)


## Summary
* After removing the data regarding Thomas High School 9th graders and recalculating all the averages and percentages, no real divergence was found. The percentages and scores varied slighlty, but not in a sense that it could suggest the data impacted the results.
* The data shows that a higher budget per student does not mean better scores. The schools that perfomed better were in the two lower budget per student ranges.
* The research also reveals that larger schools do not perform as well as small or medium ones. While small and medium schools reach 90% in overall passing, large schools do not even reach 60%.
* Charter schools perform better than district units. Once again, the number is 90% for Charter and 54% for District.