# School District Analysis
Analyze data from a school district and provide insights



## Overview of Analysis

Due to potential academic dishonesty, the Freshman class at Thomas High School (THS) has had its test scores voided. The purpose of this analysis will be to determine the impact of having these scores thrown out.



## Results of Analysis

The results of the School District Analysis changed significantly due to the potential academic dishonesty over at THS. We'll take a deep dive into several different metrics below and make before-and-after comparisons.

- The **district summary** did not change all that much. This is due to the relatively small amount of test scores that were thrown out (461) compared to the total number of student in the district (39,170).

  **Before Potential Academic Dishonesty (PAD):**

  ![district_summary_before](https://github.com/cdeanatx/School_District_Analysis/blob/main/Analysis_Images/district_summary_before.png)

  **After PAD:**

  ![district_summary_after](https://github.com/cdeanatx/School_District_Analysis/blob/main/Analysis_Images/district_summary_after.png)

- The **school summary** was not significantly impacted by the PAD. The per school statistics did not change at all, aside from THS, who experienced marginal decreases across the board in scores and passing rates.

- Despite the marginal decreases in each metric for THS, their overall **performance relative to other schools** was unaffected when measured by overall passing rate. Below are images of the school summary DataFrame, sorted by overall passing rate:

  **Before PAD:**

  ![school_summary_before](https://github.com/cdeanatx/School_District_Analysis/blob/main/Analysis_Images/school_summary_before.png)

  **After PAD:**

  ![school_summary_after](https://github.com/cdeanatx/School_District_Analysis/blob/main/Analysis_Images/school_summary_after.png)

- **Math and reading scores by grade** were only affected for the THS freshman class. Since none of the THS freshman class' scores were counted, they do not have valid averages and the "after" DataFrame returns `nan`.

|            |                             Math                             |                           Reading                            |
| :--------- | :----------------------------------------------------------: | :----------------------------------------------------------: |
| Before PAD | ![math_by_grade_before](https://github.com/cdeanatx/School_District_Analysis/blob/main/Analysis_Images/math_by_grade_before.png) | ![read_by_grade_before](https://github.com/cdeanatx/School_District_Analysis/blob/main/Analysis_Images/read_by_grade_before.png) |
| After PAD  | ![math_by_grade_after](https://github.com/cdeanatx/School_District_Analysis/blob/main/Analysis_Images/math_by_grade_after.png) | ![read_by_grade_after](https://github.com/cdeanatx/School_District_Analysis/blob/main/Analysis_Images/read_by_grade_after.png) |

- **Scores by school spending** were unaffected up to the level of precision included in the DataFrame, that is, to the tenths place for Average Scores and the nearest whole number for Passing Percentages. Both the "before PAD" and "after PAD" look like this:

  ![scores_by_spending](https://github.com/cdeanatx/School_District_Analysis/blob/main/Analysis_Images/scores_by_spending.png)

- **Scores by school size** were also unaffected up to the level of precision included in the DataFrame:

  ![scores_by_size](https://github.com/cdeanatx/School_District_Analysis/blob/main/Analysis_Images/scores_by_size.png)

- **Scores by school type** were also unaffected up to the level of precision included in the DataFrame:

  ![scores_by_type](https://github.com/cdeanatx/School_District_Analysis/blob/main/Analysis_Images/scores_by_type.png)

  

## Summary of Analysis

Despite having 461 students' scores removed from the dataset, the impact on the school district's summary was minimal. This is because the average of the 9<sup>th</sup> grade scores at THS that were thrown out were **almost identical** to the average of the 10<sup>th</sup>-12<sup>th</sup> grade scores at THS.

When we make comparisons at the district level (scores by spending/school size/school type), Thomas High School is considered as a part of a whole. Since THS's **averages** remained almost the same, the absence of the 9<sup>th</sup> grade data became inconsequential at the macro level. There were, however, a few things that changed:

1. THS's average math score dropped by about 0.07%.
2. THS's average reading score rose by about 0.05%.
3. The percentage of THS students that passed math dropped by about 0.09%.
4. The percentage of THS students that passed reading dropped by about 0.29%.
5. The percentage of THS students that passed both math and reading dropped by about 0.32%.
