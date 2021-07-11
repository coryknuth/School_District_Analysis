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

##### Original Data
![per_school_summary_original](https://github.com/coryknuth/school_district_analysis/blob/9046932ce3cc5ae7dd823842eebb2c8e6909d0d9/Resources/per_school_summary_original.png)

##### Cleaned Data
![per_school_summary_cleaned](https://github.com/coryknuth/school_district_analysis/blob/9046932ce3cc5ae7dd823842eebb2c8e6909d0d9/Resources/per_school_summary_cleaned.png)

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

In the original data, Thomas High School ranked #2 in overall passing percent for the district. After the data cleaning, while Thomas High School's overall passing percent was reduced by roughly 0.3%, Thomas maintained 2nd overall ranking for the district.

##### Original Data
![top_5_original](https://github.com/coryknuth/school_district_analysis/blob/9046932ce3cc5ae7dd823842eebb2c8e6909d0d9/Resources/top_5_original.png)

##### Cleaned Data
![top_5_cleaned](https://github.com/coryknuth/school_district_analysis/blob/9046932ce3cc5ae7dd823842eebb2c8e6909d0d9/Resources/top_5_cleaned.png)


### How does replacing the ninth-grade scores affect the following:

#### Math and reading scores by grade

Our solution to the tampered scores was to drop them altogether, replacing all Thomas 9th grade scores with N/A values. Because of this the only grade and school affected were the Thomas High 9th graders as shown.

##### Original Data

![math_by_grade_original](https://github.com/coryknuth/school_district_analysis/blob/5562b7a2c11e0f6a71be0b88fb14853aa70641e5/Resources/math_by_grade_original.png)

##### Cleaned Data

![math_by_grade_cleaned](https://github.com/coryknuth/school_district_analysis/blob/5562b7a2c11e0f6a71be0b88fb14853aa70641e5/Resources/math_by_grade_cleaned.png)
  
  
#### Scores by school spending

We found very slight changes to scores for the $630-$644 category that Thomas High School is in after correcting for the tampered data. However, with our final data for presentation being precise only to one tenth, these very slight changes didn't impact the final results.

##### Original
<img src="https://github.com/coryknuth/school_district_analysis/blob/95ac2bdcb35f267b0e74260f24325cfcabec04bf/Resources/average_by_spending_original_fixed.png" width="1000">

##### Cleaned
<img src="https://github.com/coryknuth/school_district_analysis/blob/0e68244354ca658743ee044a603ab8a266e32f59/Resources/average_by_spending_cleaned_fixed.png" width="1000">

#### Scores by school size

Much the same as with spending, as we look at the scores broken down by school size into categories, we saw fractional changes from cleaning the fraudulent scores. The changes were less than a tenth so they didn't impact our final results here since our final chart is only precise to one tenth.

##### Original
![average_by_size_original](https://github.com/coryknuth/school_district_analysis/blob/87d8abfcf5719d97bd4859fa281810f8928fbc33/Resources/average_by_size_original.png)

##### Cleaned
![average_by_size_cleaned](https://github.com/coryknuth/school_district_analysis/blob/87d8abfcf5719d97bd4859fa281810f8928fbc33/Resources/average_by_size_cleaned.png)


#### Scores by school type

We found similiar results when analyzing by school type. The differences in scores for both charter schools and district schools don't register in our data with one tenth precision.

##### Original
![average_by_type_original](https://github.com/coryknuth/school_district_analysis/blob/87d8abfcf5719d97bd4859fa281810f8928fbc33/Resources/average_by_type_original.png)

##### Cleaned
![average_by_type_cleaned](https://github.com/coryknuth/school_district_analysis/blob/87d8abfcf5719d97bd4859fa281810f8928fbc33/Resources/average_by_type_cleaned.png)


### Summary

Thankfully, the amount of data that was compromised relative to the entire dataset was extremely small. We saw the most impact to the average scores for Thomas High School itself. we saw Math and Reading averages, as well as percent passing both subjects and overall were impacted with 0.3% from the original. These changes became even smaller when you analyze at the district level between all schools and students. We found changes measured only in hundreths to average scores regardless of how the data was categorized. We broke it down by spending, size, and school type, and saw little to no impact to the final data to be presented.
