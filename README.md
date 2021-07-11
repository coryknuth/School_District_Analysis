# School District Analysis

We were tasked with analyzing a collection of data from the local school district, comparing test scores against school characteristics like size and spending to help the district leadership make budgetary decisions about next school year. One issue we ran into before completing our analysis was evidence of tampering with test score numbers relating to one grade, at one school. In order to prevent this from polluting the dataset, we removed these fraudulent scores from the data, and re-ran the analysis. We then compared the first dataset, which included the fraudulent scores, against the new data which had been cleaned.

### How is the district summary affected?

We found that, due to the very small amount of students scores that were affected by the tampering, there was hardly any impact felt at the district summary level. Here is the original data.

![district_summary_original](https://github.com/coryknuth/school_district_analysis/blob/9046932ce3cc5ae7dd823842eebb2c8e6909d0d9/Resources/district_summary_original.png)

And here is the same table, scrubbed for the tampered scores.

![district_summary_cleaned](https://github.com/coryknuth/school_district_analysis/blob/9046932ce3cc5ae7dd823842eebb2c8e6909d0d9/Resources/district_summary_cleaned.png)

As shown, there was a 0.1 decrease in the percent passing overall, and the average math score. There was a 0.2 decrease in the percent passing math, and a 0.3 decrease in percent passing reading. Again, the number of scores compared to the entire district count that were fraudulent was a very small fraction.

### How is the school summary affected?

As we compare the school summaries before and after data cleaning, you'll see the impact was tiny, but measurable to the overall scores for Thomas High School.

Original Data
![per_school_summary_original](https://github.com/coryknuth/school_district_analysis/blob/9046932ce3cc5ae7dd823842eebb2c8e6909d0d9/Resources/per_school_summary_original.png)

Cleaned Data
![per_school_summary_cleaned](https://github.com/coryknuth/school_district_analysis/blob/9046932ce3cc5ae7dd823842eebb2c8e6909d0d9/Resources/per_school_summary_cleaned.png)

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

In the original data, Thomas High School ranked #2 in overall passing percent for the district. After the data cleaning, while Thomas High School's overall passing percent was reduced by roughly 0.3%, Thomas maintained 2nd overall ranking for the district.

Original Data
![top_5_original](https://github.com/coryknuth/school_district_analysis/blob/9046932ce3cc5ae7dd823842eebb2c8e6909d0d9/Resources/top_5_original.png)

Cleaned Data
![top_5_cleaned](https://github.com/coryknuth/school_district_analysis/blob/9046932ce3cc5ae7dd823842eebb2c8e6909d0d9/Resources/top_5_cleaned.png)


### How does replacing the ninth-grade scores affect the following:

#### Math and reading scores by grade

Our solution to the tampered scores was to drop them altogether, replacing all Thomas 9th grade scores with N/A values. Because of this the only grade and school affected were the Thomas High 9th graders as shown.

Original Data
![math_by_grade_original](https://github.com/coryknuth/school_district_analysis/blob/5562b7a2c11e0f6a71be0b88fb14853aa70641e5/Resources/math_by_grade_original.png)

Cleaned Data
![math_by_grade_cleaned](https://github.com/coryknuth/school_district_analysis/blob/5562b7a2c11e0f6a71be0b88fb14853aa70641e5/Resources/math_by_grade_cleaned.png)
  
#### Scores by school spending



#### Scores by school size



#### Scores by school type


Summary: Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
