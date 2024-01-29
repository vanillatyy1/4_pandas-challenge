# 4_pandas-challenge

You are the new Chief Data Scientist for your city's school district, and you are helping the school board and mayor make strategic decisions regarding future school budgets and priorities. 

Download the Module 4 Challenge files,
- Open PyCitySchools & check out the sample solution called PyCitySchools_starter.ipynb
- Review the two Resouces file, schools_complete & students_complete

# Part 1.
District Summary
- Perform the necessary calculations and then create a high-level snapshot of the district's key metrics in a DataFrame.

School Summary:
- Perform the necessary calculations and then create a DataFrame that summarizes key metrics about each school.

# Part 2.
a) Write a summary to showcase the obvious trend, and 

b) Draws two correct conclusions or comparisons from the calculations 


# District Summary:
There are 15 schools in the district with a total number of 39,170 students.

The average math score is 78.99, and the average reading score is 81.88.

The percentage of students who passed math (math scores greather than or equal to 70) is 75%, the percentage of students who passed reading (greather than or equal to 70) is 86% and the percentage of students that passed math and reading is 65%.


# School Summary:

# Charter Schools outperforms District Schools

On average, students at Charter Schools do better than students at District Schools. The % of Overall Passing in Charter School is 90%, but the % of Overall Passing is only hits 54%. 


Students have a higher average math and reading score in Charter Schools, and the % passing on either subject is well above 90%.

Students in District Schools, however, only have an average math school of 76.96, and average reading score of 80.97, both of which are lower than the district average. 


The Highest-Performing Schools by Percentage of Overall Passing (Top 5) are Charter Schools [Cabrera High School, Thomas High School, Griffin High School, Wilson High School, Pena High School], and Lowest-Performing Schools by Percentage of Overall Passing (Bottom 5) are District Schools [Rodriguez High School, Figueroa High School, Huang High School, Hernandez High School, Johnson High School] 

Therefore, based on the provided data, we could suggest that the school type played an important factor in determining academic success. 


# Budget v.s. Academic Performance

Based on the provided data, it does not seem like a higher spending range per student will always result in better math or reading score. In fact, with per-student budget increases, there is a noticeable decline in academic performance. For example, school(s) with a lowest spending ranges per student, display a higher % of overall passing (90%) compared to School(s) with spending ranges per student of $645-680, which only have 54% of overall passing.

And reviewing the Scores by School Spending, Schools with a higher total school budget also has a lower average math score and % passing math, compared to schools with a lower total school budget. 

Further analysis would be beneficial to explore whether higher funding contributes to academic success and better quality education, as there are certain limition to the data set to draw a definite conclusion.
For example, the dataset lacks information about teaching methodologies, school culture, parental involvement, community support, and detailed financial information in terms of how the funds are utilized within schools. Understanding these factors is important for a more comprehensive assessment of the relationship between funding and educational outcomes, and the overall educational landscape. 

