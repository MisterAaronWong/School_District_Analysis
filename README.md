# School_District_Analysis

## Overview of the School District Analysis
The purpose of this analysis was to re-examine the original data report sent to Maria and her supervisor because the school board notified them of possible academic dishonesty for the reported math and reading scores of ninth graders in one particular school -- Thomas High School. Though the school board has not completely confirmed the extent of the academic dishonesty, Maria requested that all math and reading scores for ninth graders at Thomas High School be replaced with "NaN" ("Not a Number"), while keeping the rest of the data intact. After the score data for Thomas High School was adjusted as requested, the school district analysis was repeated once more to analyze how those adjustments affected the overall analysis. 

## Results

### How is the district summary affected?
Prior to the adjustment, the district summary showed the data as seen below:

![original_district](Resources/original_district.png)

After the adjustment was made, the impact appears to be miniscule. Ninth-graders at Thomas High School represented a total count of 461 students. The removal of their scores from the rest of the 39,170 students' scores that encompass all grade levels at all other school in the district did not seem to have much effect. In fact, the change resulted in a less than 1% difference, as the average math/reading scores as well as the % passing math/reading data all still round to the same whole number. Refer to the below image for the adjusted dataset:

![amended_district](Resources/amended_district.png)

### How is the school summary affected?
When examining how the summary was affected distinctly for Thomas High School, the adjustment showed a much larger impact to the data. Before changing the ninth grade scores to null for Thomas High School, the score percentages were all quite low in the 60s, with the overall passing rate at 65%. Refer below:

![original_thomas](Resources/original_thomas.png)

After factoring out the ninth graders' scores at Thomas High School though, the overall passing percentage rate increased to nearly 91%. The passing math and reading percentages also individually increased sharply to 93% and 97%, respectively. In other words, the low scores for Thomas High School's 9th graders heavily skewed and impacted the rest of the school's data. See below:

![amended_thomas](Resources/amended_thomas.png)

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
In the original dataset prior to discarding the math and reading scores for the 9th graders at Thomas High School, Thomas High School's overall passing percentage of 65% ranked squarely in the middle of the pack at #8 amongst the fifteen schools in the district. See below for the original analysis:

![original_rank](Resources/original_rank.png)

After replacing the scores with only 10th-12th grade scores, with the new overall passing percentage at nearly 91%, Thomas High School jump to the #2 ranking amongst the district. See below:

![new_rank](Resources/new_rank.png)

### How replacing the ninth-grade scores affects the following:
#### Math and reading scores by grade
Thomas High School originally reported 83.6 for their 9th graders' average math score and 83.7 for their 9th graders' average reading score. Replacing the ninth-grade scores with NaN only affected the school's overall average but did not affect the individual averages for the other grade levels. Only the 9th grade math and reading scores at Thomas High School were changed to NaN. Therefore, all the score averages for other grade levels at all other schools including Thomas High School remained the same.

Math Scores by Grade:

![new_math](Resources/new_math.png)

Reading Scores by Grade:

![new_reading](Resources/new_reading.png)

#### Scores by school spending
Thomas High School falls into the $630-$644 bin of student spending ranges. There was minimal impact to the data. The average math and reading scores still round to the same whole number, but the % Passing Math, % Passing Reading, and % Overall Passing data saw slight shifts. However, these changes would no be noticeable unless the numbers are formatted to the hundreths place. See below:

Original:

![spending_original](Resources/original_spending.png)

Adjusted:

![spending_new](Resources/new_spending.png)

#### Scores by school size
Based on Thomas High School's population, it is considered a medium sized school. There was a slight but barely noticeable increase in the passing percentage data. This change would not be noticeable unless the numbers are formatted to display to the hundreths place. The averages for math and reading remained the same. However, the passing math, reading, and overall passing percentages all saw an extremely slight reduction. See below:
Original:

![size_original](Resources/original_size.png)

Adjusted:

![size_new](Resources/new_size.png)

#### Scores by school type
Thomas High School is a charter school. Likewise with school spending and school size, there was a minor but barely noticeable change that could only be discerned after formatting the data to the hundreths place. Once again, the averages for math and reading remained the same. However, the passing math percentage, passing reading percentage, and overall passing percentage all had an extremely slight reduction. See below:
Original:

![type_original](Resources/original_type.png)

Adjusted:

![type_new](Resources/new_type.png)

## Summary
In summary, the replacing of NaNs for reading and math scores at Thomas High School had minimal impact on the overall scores and passing percentages when looked at within the district as a whole. However, there was significant impact to the data when comparing Thomas High School's new adjusted data to the rest of the schools' data individually. The changes resulted in a significant increase for Thomas High School's passing math percentage, passing reading percentage, and the overall passing percentage. Additionally, as a result of this increase in overall passing percentage, Thomas High School's new values changed its position amongst the other schools in the district. Most notably, its ranking amongst the rest of the schools increased from its original #8 ranking to the #2 ranking, making it the high school with the second highest overall passing percentage within the district, behind only Cabrera High School. Most likely, if any academic dishonesty occurred, this is where it was concentrated.

However, all the other impacts to the data were minor and hardly noticeable. There were slight reductions in the school spending, school size and school type. However this would not be seen unless formatting the % Passing Math, % Passing Reading, and % Overall Passing data to the hundreths place. If only whole percentages are used, the changes would not even be noticed. This indicates that the nulling of scores in one grade level for a single school does not have much influence on the rest of the data.
