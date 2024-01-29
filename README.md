# 4_pandas-challenge

## Introduction

You are the new Chief Data Scientist for your city's school district, and you are helping the school board and mayor make strategic decisions regarding future school budgets and priorities. 

Download the Module 4 Challenge files,
- Open PyCitySchools & check out the sample solution called PyCitySchools_starter.ipynb
- Review the two Resouces file, schools_complete & students_complete

Part 1.
- Perform the necessary calculations on District & School Summary, and then create a high-level snapshot/ DataFrames of the key metrics.
- (The final calculations are store in PyCitySchools_final.ipynb within the PyCitySchools folder)

Part 2.
- Write a summary to showcase the obvious trend, and 
- Draws two correct conclusions or comparisons from the calculations 


### District Summary:
There are 15 schools in the district with a total number of 39,170 students.
The average math score is 78.99, and the average reading score is 81.88.
The percentage of students who passed math (math scores greather than or equal to 70) is 75%, the percentage of students who passed reading (greather than or equal to 70) is 86% and the percentage of students that passed math and reading is 65%.

### School Summary:
#### Charter Schools outperforms District Schools

- On average, students at Charter Schools do better than students at District Schools. The % of Overall Passing in Charter School is 90%, but the % of Overall Passing is only hits 54%. 
- Students have a higher average math and reading score in Charter Schools, and the % passing on either subject is well above 90%.
- Students in District Schools, however, only have an average math school of 76.96, and average reading score of 80.97, both of which are lower than the district average.

| School Type | Average Math Score | Average Reading Score | % Passing Math | % Passing Reading | % Overall Passing |
|-------------|--------------------|-----------------------|----------------|-------------------|-------------------|
| Charter     | 83.473852          | 83.896421             | 93.620830      | 96.586489         | 90.432244         |
| District    | 76.956733          | 80.966636             | 66.548453      | 80.799062         | 53.672208         |

- The Highest-Performing Schools by Percentage of Overall Passing (Top 5) are Charter Schools [Cabrera High School, Thomas High School, Griffin High School, Wilson High School, Pena High School], and Lowest-Performing Schools by Percentage of Overall Passing (Bottom 5) are District Schools [Rodriguez High School, Figueroa High School, Huang High School, Hernandez High School, Johnson High School] 
- Therefore, based on the provided data, we could suggest that the school type played an important factor in determining academic success.
  
### Highest-Performing Schools by Percentage of Overall Passing

|                     | School Type | Total Students | Total School Budget | Per Student Budget | Average Math Score | Average Reading Score | % Passing Math | % Passing Reading | % Overall Passing |        School Size |
|--------------------:|------------:|---------------:|--------------------:|-------------------:|-------------------:|----------------------:|---------------:|------------------:|------------------:|-------------------:|
| Cabrera High School |     Charter |           1858 |       $1,081,356.00 |            $582.00 |          83.061895 |             83.975780 |      94.133477 |         97.039828 |         91.334769 | Medium (1000-2000) |
|  Thomas High School |     Charter |           1635 |       $1,043,130.00 |            $638.00 |          83.418349 |             83.848930 |      93.272171 |         97.308869 |         90.948012 | Medium (1000-2000) |
| Griffin High School |     Charter |           1468 |         $917,500.00 |            $625.00 |          83.351499 |             83.816757 |      93.392371 |         97.138965 |         90.599455 | Medium (1000-2000) |
|  Wilson High School |     Charter |           2283 |       $1,319,574.00 |            $578.00 |          83.274201 |             83.989488 |      93.867718 |         96.539641 |         90.582567 |  Large (2000-5000) |
|    Pena High School |     Charter |            962 |         $585,858.00 |            $609.00 |          83.839917 |             84.044699 |      94.594595 |         95.945946 |         90.540541 |      Small (<1000) |

### Lowest-Performing Schools by Percentage of Overall Passing

|                       | School Type | Total Students | Total School Budget | Per Student Budget | Average Math Score | Average Reading Score | % Passing Math | % Passing Reading | % Overall Passing |        School Size |
|----------------------:|------------:|---------------:|--------------------:|-------------------:|-------------------:|----------------------:|---------------:|------------------:|------------------:|-------------------:|
| Rodriguez High School |    District |           3999 |       $2,547,363.00 |            $637.00 |          76.842711 |             80.744686 |      66.366592 |         80.220055 |         52.988247 | Medium (1000-2000) |
|  Figueroa High School |    District |           2949 |       $1,884,411.00 |            $639.00 |          76.711767 |             81.158020 |      65.988471 |         80.739234 |         53.204476 | Medium (1000-2000) |
|     Huang High School |    District |           2917 |       $1,910,635.00 |            $655.00 |          76.629414 |             81.182722 |      65.683922 |         81.316421 |         53.513884 | Medium (1000-2000) |
| Hernandez High School |    District |           4635 |       $3,022,020.00 |            $652.00 |          77.289752 |             80.934412 |      66.752967 |         80.862999 |         53.527508 |  Large (2000-5000) |
|   Johnson High School |    District |           4761 |       $3,094,650.00 |            $650.00 |          77.072464 |             80.966394 |      66.057551 |         81.222432 |         53.539172 |      Small (<1000) |

#### Budget v.s. Academic Performance

Based on the provided data, it does not seem like a higher spending range per student will always result in better math or reading score. In fact, with per-student budget increases, there is a noticeable decline in academic performance. For example, school(s) with a lowest spending ranges per student, display a higher % of overall passing (90%) compared to School(s) with spending ranges per student of $645-680, which only have 54% of overall passing.

|                               | Average Math Score | Average Reading Score | % Passing Math | % Passing Reading | % Overall Passing |
|------------------------------:|-------------------:|----------------------:|---------------:|------------------:|------------------:|
| Spending Ranges (Per Student) |                    |                       |                |                   |                   |
|                         <$585 |          83.455399 |             83.933814 |      93.460096 |         96.610877 |         90.369459 |
|                      $585-630 |          81.899826 |             83.155286 |      87.133538 |         92.718205 |         81.418596 |
|                      $630-645 |          78.518855 |             81.624473 |      73.484209 |         84.391793 |         62.857656 |
|                      $645-680 |          76.997210 |             81.027843 |      66.164813 |         81.133951 |         53.526855 |

And reviewing the Scores by School Spending, Schools with a higher total school budget also has a lower average math score and % passing math, compared to schools with a lower total school budget. 

Further analysis would be beneficial to explore whether higher funding contributes to academic success and better quality education, as there are certain limition to the data set to draw a definite conclusion.
For example, the dataset lacks information about teaching methodologies, school culture, parental involvement, community support, and detailed financial information in terms of how the funds are utilized within schools. Understanding these factors is important for a more comprehensive assessment of the relationship between funding and educational outcomes, and the overall educational landscape. 

#### Reference
Markdown table generator (converting tables into Markdown): https://www.tablesgenerator.com/markdown_tables
