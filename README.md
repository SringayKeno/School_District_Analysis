# School_District_Analysis

## Overview of the School District Analysis: Purpose of this Analysis

Maria, the Chief Data Scientist for a city school district is tasked with preparing all standardized test data for analysis, reporting and presentation to provide insights about performance, trends and patterns. These insights are used to inform discussions and strategic decisions at the school and district level. I assisted Maria on analyzing data on student funding and students stanardized test scores. I was given access to every students math and reading scores as well as information on the schools they attend. My task was to aggregate the data and showcase the trends in school performance. This analysis will assist the schoolboard and Superintendant in making decisions in regading to school budgets and priorities.


## Results: 

After completion of the first analysis, the school board notified Maria that the students_complete.csv file (one of the files we drew data from) shows evidence of academic dishonesty; specifically, reading and math grades for Thomas High School ninth graders appear to have been altered. Although the school board did not know the full extent of the academic dishonesty, they wanted to uphold state-testing standards and turned to Maria for help. Maria asked to replace the math and reading scores for Thomas High School with NaNs (not a number) while keeping the rest of the data intact. Once replaced I repeated the school district analysis.

### How the District Summary is Affected?

With the math and reading scores for Thomas High School replaced with NaNs the passing reading, passing math and the overall passing percentages all dropped approximately 1 percent for the district. See images 1 and 2 below.

(Image 1) district summary after first analysis
<img width="800" alt="district_summary_initial" src="https://user-images.githubusercontent.com/102890151/166126312-31d4b355-ebf1-48a9-a08d-30509cbfd886.png">

(Image 2) district summary after math and reading scores for Thomas High School ninth graders were replaced with NaNs 
<img width="800" alt="district_summary" src="https://user-images.githubusercontent.com/102890151/166126314-2803a439-f54c-4345-abb9-265421748e4f.png">

### How the school summary is affected?

Thomas High Schools % passing math (3rd column from right) % passing reading and % overall passing (last column on right) all decreased dramatically after the math and reading scores for Thomas High School ninth graders were replaced with NaNs. Removing the 9th grade students from the data set dropped the overall passing rate from 91% to 65%.

Image 3. Thomas High Schools % and scores after original analysis
<img width="800" alt="per_school_summary_df_first" src="https://user-images.githubusercontent.com/102890151/166130709-50811062-8d21-4e17-b731-380c205fa855.png">

Image 4. Thomas High Schools % and scores after adjusted analysis
<img width="800" alt="per_school_summary_df_after" src="https://user-images.githubusercontent.com/102890151/166130712-cf7a4698-6d01-463e-9223-75628b9e20b8.png">

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

In the original analysis, Thomas High School was ranked 2nd (See image 5 , below) in % of overall passing scores. After adjusting the 9th grade data, Thomas High ranked in the right in the middle of 15 campuses at #8 with it's 65 in % of overall passing scores.

Image 5

<img width="600" alt="school_summary_overall_passing_initial" src="https://user-images.githubusercontent.com/102890151/166131537-3517810b-855e-4ec2-bd74-31d03193b221.png">


### How does replacing the ninth-grade scores affect the following:
### Math and reading scores by grade
### Scores by school spending
### Scores by school size
### Scores by school type

Charter vs. District Schools
Charter schools generally performed better than District schools in this analysis. The top five schools with the highest overall passing percentages are all Charter schools, whereas the bottom five are all District Schools. Charter schools in this dataset were typically characterized as "Small" and "Medium" size schools. As seen in the DataFrame below, Charter schools have a 36% higher overall passing percentage than District schools.


## Summary: 
### Four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.

Having to replace the ninth graders' scores at Thomas High caused the overall passing percentages and average scores to drop. The district as a whole has also had its average math and reading scores decrease, as well as the overall passing percentage for students.
