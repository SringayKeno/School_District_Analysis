# School_District_Analysis

## Overview of the School District Analysis: Purpose of this Analysis

Maria, the Chief Data Scientist for a city school district is tasked with preparing all standardized test data for analysis, reporting and presentation to provide insights about performance, trends and patterns. These insights are used to inform discussions and strategic decisions at the school and district level. I assisted Maria on analyzing data on student funding and students stanardized test scores. I was given access to every students math and reading scores as well as information on the schools they attend. My task was to aggregate the data and showcase the trends in school performance. This analysis will assist the schoolboard and Superintendant in making decisions in regading to school budgets and priorities.


## Results: 

After completion of the first analysis, the school board notified Maria that the students_complete.csv file (one of the files we drew data from) shows evidence of academic dishonesty; specifically, reading and math grades for Thomas High School ninth graders appear to have been altered. Although the school board did not know the full extent of the academic dishonesty, they wanted to uphold state-testing standards and turned to Maria for help. Maria asked to replace the math and reading scores for Thomas High School with NaNs (not a number) while keeping the rest of the data intact. Once replaced I repeated the school district analysis.

### How the District Summary was Affected?

With the math and reading scores for Thomas High School's ninth grade replaced with NaNs the passing reading, passing math and the overall passing percentages all dropped approximately 1 percent for the district. See images 1 and 2 below. Thomas High's ninth grade consisted of 461 students.

(image 1) district summary after first analysis
<img width="800" alt="district_summary_initial" src="https://user-images.githubusercontent.com/102890151/166126312-31d4b355-ebf1-48a9-a08d-30509cbfd886.png">

(image 2) district summary after math and reading scores for Thomas High School ninth graders were replaced with NaNs 
<img width="800" alt="district_summary" src="https://user-images.githubusercontent.com/102890151/166126314-2803a439-f54c-4345-abb9-265421748e4f.png">

### How the school summary was affected?

Thomas High Schools % passing math (3rd column from right) % passing reading and % overall passing (last column on right) all decreased dramatically after the math and reading scores for Thomas High School ninth graders were replaced with NaNs. Removing the 9th grade students from the data set dropped the overall passing rate from 91% to 65%.

image 3. Thomas High Schools % and scores after original analysis
<img width="800" alt="per_school_summary_df_first" src="https://user-images.githubusercontent.com/102890151/166130709-50811062-8d21-4e17-b731-380c205fa855.png">

image 4. Thomas High Schools % and scores after adjusted analysis
<img width="800" alt="per_school_summary_df_after" src="https://user-images.githubusercontent.com/102890151/166130712-cf7a4698-6d01-463e-9223-75628b9e20b8.png">

### How did replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

In the original analysis, Thomas High School was ranked 2nd (See image 5, below) in % of overall passing scores. After adjusting the 9th grade data, Thomas High ranked in the middle of the 15 campuses at rank #8 with it's 65 in % of overall passing scores.

image 5. In initial analysis Thomas High School was ranked 2nd in % overall passing scores

<img width="700" alt="school_summary_overall_passing_initial" src="https://user-images.githubusercontent.com/102890151/166131537-3517810b-855e-4ec2-bd74-31d03193b221.png">

### How did replacing the ninth-grade scores affect the following?
- Math and reading scores by grade

In the original analysis, Thomas High had an 83.6 math average and an 83.7 reading average for those 9th grade tests. After adjusted analysis, the scores have been replaced with null values (NaN)

image 6. Thomas High Schools ninth grades reading score shown as NAN in adjusted analysis

<img width="350" alt="thomas_reading_nan" src="https://user-images.githubusercontent.com/102890151/166132074-338ca2f9-3ccb-4517-89d2-189b5da2373c.png">


- Scores by school spending

Thomas High School was in the $630-$644/student spending range. Again, the hundredths place was needed to see the changes in the score by spending (images 7 and 8).

image 7. initial analysis

<img width="719" alt="spending_initial" src="https://user-images.githubusercontent.com/102890151/166153707-7e4af54e-70a0-4610-b38b-75895de43a1d.png">

image 8. adjusted analysis

<img width="724" alt="spendingadjusted" src="https://user-images.githubusercontent.com/102890151/166153710-9d7ac0cc-14d3-4d4b-b54d-bd95ae0caad6.png">


- Scores by school size

Thomas High School is defined as a medium sized school. The hundredths place would have been needed to see the nominal changes in the passing math, passing reading and over passing columns (images 9 and 10).

image 9. initial analysis

<img width="700" alt="size_initial" src="https://user-images.githubusercontent.com/102890151/166152726-952d6f1a-6a06-4cd4-abab-1bc746f1368c.png">

image 10. adjusted analysis

<img width="700" alt="size_adjustd" src="https://user-images.githubusercontent.com/102890151/166152729-ef465a80-2f0e-4566-9833-c70a04fa7cba.png">


- Scores by school type

Replacing the ninth-grade scores from Thomas High School did not affect the initial summary for scores by school type. There is a major trend in the scores by school type however. Charter schools in general performed better than District schools. The top five schools with the highest overall passing percentages are all Charter schools. The bottom five schools are all District Schools.

image 11. Initial analysis (schools by type)

<img width="650" alt="type_initial" src="https://user-images.githubusercontent.com/102890151/166152144-97f79248-cc5f-4260-9073-b51e744d9e92.png">

image 12. Adjusted analysis (schools by type)

<img width="650" alt="type_adjusted" src="https://user-images.githubusercontent.com/102890151/166152250-0e234ffe-ff63-4176-9711-397c8679c852.png">

## Summary: 
### Four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.

There were a number of changes. Having to replace the ninth graders' scores at Thomas High caused (1) the overall passing percentages and average scores to drop at the school. (2) The district as a whole has also had its average math and reading scores decrease, as well as the overall passing percentage for students. (3) Data at the ninth grade level will now show as "NaN" in reports for Thomas High. (4) Thomas High School's ranking dropped from 2nd to 8th in the district of 15 campuses with the removal of the ninth grade's testing scores.
