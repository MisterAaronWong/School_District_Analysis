# School_District_Analysis

## Overview of the School District Analysis
The purpose of this analysis was to re-examine the original data report sent to Maria and her supervisor because the school board notified them of possible academic dishonesty for the reported math and reading scores of ninth graders in one particular school -- Thomas High School. Though the school board has not completely confirmed the extent of the academic dishonesty, Maria requested that all math and reading scores for ninth graders at Thomas High School be replaced with "NaN" ("Not a Number"), while keepiing the rest of the data intact. After the score data for Thomas High School was adjusted as requested, the school district analysis was repeated once more to analyze how those adjustments affected the overall analysis. 

## Results
Using bulleted lists and images of DataFrames as support, address the following questions.
### How is the district summary affected?
Prior to the adjustment, the district summary showed the data as seen below:
![original_district](Resources/original_district.png)

REDO*** After the adjustment was made, the impact seems miniscule. When factored into the rest of the student dataset, the removal of 461 scores from 9th graders at Thomas High School from the rest of the 39,170 student scores that encompass all grade levels at all other school in the district, the results don't appear to move much. In fact, the change resulted in a less than 1% difference, as the average math/reading scores as well as the % passing math/reading data still rounds to the same whole numer. Refer to the below image for the adjusted dataset:
![amended_district](Resources/amended_district.png)

### How is the school summary affected?
When examining how the summary summary was affected for Thomas High School though, the adjustment showed a much larger impact to the data. Before changing the ninth grade scores to null for Thomas High School, the overall passing rate was 65%. Refer below:
![original_thomas](Resources/original_thomas.png)

After factoring out the ninth graders' scores at Thomas High School though, the overall passing percentage rate increased to nearly 91%. The passing math and reading percentages also individually increased sharply to 93% and 97%, respectively. In other words, the low scores for thomas High School's 9th graders heavily skewed and impacted the rest of the school's data. See below:
![amended_thomas](Resources/amended_thomas.png)

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
In the original dataset prior to the changes, Thomas High School had the second highest overll passing percentage amongst the fifteen schools in the district. See below for the original analysis:
![original_rank](Resources/original_rack.png)

After replacing the scores, Thomas High School's overall passing percentage ranked in the middle at position #8. See below:
![new_rank](Resources/new_rank.png)

### How does replacing the ninth-grade scores affect the following:
#### Math and reading scores by grade
Replacing the ninth-grade scores for Thomas High School only affected the school's overall average but did not affect the individual averages for Thomas High School scores for the other grade levels.
Original:
![math_reading_original](Resources/math_reading_original.png)

Adjusted:
![math_reading_new](Resources/math_reading_new.png)

#### Scores by school spending
Thomas High School falls into the $630-$644 bin of stundent spending range. There was minimal to no impact on spending after changing the ninth-grade scores to NaN. See below:
Original:
![spending_original](Resources/spending_original.png)

Adjusted:
![spending_new](Resources/spending_new.png)

#### Scores by school size
Based on Thomas High School's population, it is considered a medium sized school. There was a slight but barely noticeable increase in the passing percentage data. See below:
Original:
![size_original](Resources/size_original.png)

Adjusted:
![size_new](Resources/size_new.png)

#### Scores by school type
Thomas High School is a charter school. Likewise with school spending and school size, there was a slight but barely noticeable change. See below:
Original
![type_original](Resources/type_original.png)

Adjusted:
![type_new](Resources/type_new.png)

## Summary
In summary, the replacing of NaNs for reading and math scores at Thomas High School had minimal impact on the overall scores and passing percentages when looked at within the district as a whole. However, there was significant impact to the data when comparing Thomas High School's new adjusted data to the rest of the schools' data individually. The changes resulted in a significant increase for Thomas high School's passing math percentage, passing reading ercentage, and the overall passing percentage. Additionally, as a result of this reduction in overall passing percentage, Thomas High School's new values changed its position amongst the other schools in the district. Most notably, it's ranking amongst the rest of the schools increased to the #2 ranking, making it the high school with the second highest overall passing percentage within the district, behind only Cabrera High School.

However, all the other impacts to the data were minor and hardly noticeable. There were slight reductions in the school spending, school size and school type. However this can only be seen when formatting the % Passing, % Passign Reading, and % Overall Passing data to the hundrethds place. If only whole percentages are used, the changes would not even be noticed except for ...
