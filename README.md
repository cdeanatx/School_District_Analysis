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

