# School District Analysis
Python pandas program for school district analysis

## Overview of the School district analysis

### Purpose

1. Help **Maria**, the chief data scientist for city school district present useful insights to **District School Board** and **Superintendent** by analyzing below **performance metrics** using clean **school funding** and **student test scores** data. This will help the key stakeholders in making decision regarding the district and school budgets and priorities.
2. Follow **Family Educational Rights and Privacy Act (FERPA)** and treat the data with utmost confidentiality to protect the students while working on school district analysis.
2. Re-analyze the data after disregarding **9th grade** Math and Reading scores for **Thomas high school** due to suspected Academic dishonesty
3. Provide **written analysis** on the updated School District Analyis and its effect to be provided to the **School Board**.

**Performance metrics to be provided**

	District Level:

	- Total number of students
	- Total number of schools
	- Total budget
	- Average math score
	- Average reading score
	- Percentage of students who passed math
	- Percentage of students who passed reading
	- Overall passing percentage

	School Level:

	- School name
	- School type
	- Total students
	- Total school budget
	- Per student budget
	- Average math score
	- Average reading score
	- Percentage of students who passed math
	- Percentage of students who passed reading
	- Overall passing percentage 

	Additional Metrics

	- Top 5 and bottom 5 performing schools, based on the overall passing rate
	- The average math score received by students in each grade level at each school
	- The average reading score received by students in each grade level at each school
	- School performance based on the budget per student
	- School performance based on the school size 
	- School performance based on the type of school

## Resources
Data source: schools_complete.csv, students_complete.csv
Software: Python 3.7, Pandas, Anaconda, JupyterNotebook


## Results

 - **How is the district summary affected?**
	
	Average Math Score, Passing Math %, Passing Reading%, and Overall Passing %  **decreased** by **0.1%,0.2%,0.3% and 0.1%** respectively. Average Reading Score was not impacted
	
	Before-> 
	![](https://github.com/Sheetaltkr/School_District_Analysis/blob/main/Images/District_summary_before.png)
	After-> 
	![](https://github.com/Sheetaltkr/School_District_Analysis/blob/main/Images/District_summary_after.png)

-	**How is the school summary affected?**
	
	For Thomas High School:
	Passing Math %, Passing Reading%, and Overall Passing % **decreased** by **26%, 27%,26%** respectively  Average Math Score and Average Reading Score were not impacted

	Before-> 
	![](https://github.com/Sheetaltkr/School_District_Analysis/blob/main/Images/School_summary_before.png)
	After-> 
	![](https://github.com/Sheetaltkr/School_District_Analysis/blob/main/Images/School_summary_after.png)

	
- **How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?**

	**Before replacement** Thomas High School showed up in Top 5 schools at second position for Overall Passing % with **90.9%.**
				![](https://github.com/Sheetaltkr/School_District_Analysis/blob/main/Images/Top_5_schools_before_replace.png)
	
	**After replacing 9th grade math and reading scores with "NaN" values and considering the 9th grade student** count for calculating the Overall Passing % ; Thomas High School loses its position in Top 5 schools with **65%**. The top second position is taken by Griffin High School
				![](https://github.com/Sheetaltkr/School_District_Analysis/blob/main/Images/Top_5_schools_after_replace.png)
	
	**After re-calculating the Overall Passing % with 9th grade student count removed;** Thomas High School recovers its second position in Top 5 schools with a slight decrease in Overall Passing % i.e. **90.6%**
				![](https://github.com/Sheetaltkr/School_District_Analysis/blob/main/Images/Top_5_schools_after_update.png)

- **How does replacing the ninth-grade scores affect the following:**

	**- Math and reading scores by grade**

	 Math scores for 9th grade changed from 83.6% to NaN for Thomas High School
		
	 Before-> 
    ![](https://github.com/Sheetaltkr/School_District_Analysis/blob/main/Images/math_scores_by_grade_before.png)
	  After-> 
    ![](https://github.com/Sheetaltkr/School_District_Analysis/blob/main/Images/math_scores_by_grade_after.png)

    Reading scores for 9th grade changed from 83.7% to NaN for Thomas High School

	Before-> 
	![](https://github.com/Sheetaltkr/School_District_Analysis/blob/main/Images/reading_scores_by_grade_before.png)	
		After-> 
	![](https://github.com/Sheetaltkr/School_District_Analysis/blob/main/Images/reading_scores_by_grade_after.png)
	

	**- Scores by school spending**
		
	For Spending Range ($630-644) the Passing Math %, Passing Reading%, and Overall Passing % **decreased** by **6%, 7% and 7%** respectively soon after replacing 			with "NaN". However there was no impact after data for 9th grade was filtered out and re-analyzed.
	
	Before-> 
	![](https://github.com/Sheetaltkr/School_District_Analysis/blob/main/Images/scores_by_school_spending_before.png)	
	
	After replace-> 
	![](https://github.com/Sheetaltkr/School_District_Analysis/blob/main/Images/scores_by_school_spending_after_replace.png)
	
	After filtering out 9th grade ->
	![](https://github.com/Sheetaltkr/School_District_Analysis/blob/main/Images/scores_by_school_spending_after_update.png)
	
	**- Scores by school size**
		
	For Medium School Size (1000-2000) Passing Math %, Passing Reading%, and Overall Passing % **decreased** by **6%** soon after replacing with "NaN". However there 		  was no impact after data for 9th grade was filtered out and re-analyzed.
	
	Before-> 
	![](https://github.com/Sheetaltkr/School_District_Analysis/blob/main/Images/scores_by_school_size_before.png)	
	
	After replace-> 
	![](https://github.com/Sheetaltkr/School_District_Analysis/blob/main/Images/scores_by_school_size_after_replace.png)
	
	After filtering out 9th grade ->
	![](https://github.com/Sheetaltkr/School_District_Analysis/blob/main/Images/scores_by_school_size_after_update.png)
	
	**- Scores by school type**
		
	For Charter School Type Passing Math %, Passing Reading%, and Overall Passing % **decreased** by **4%,4% and 3%** respectively soon after replacing. However there was no impact after data for 9th grade was filtered out and re-analyzed.
	
	Before-> 
	![](https://github.com/Sheetaltkr/School_District_Analysis/blob/main/Images/scores_by_school_type_before.png)	
	
	After replace-> 
	![](https://github.com/Sheetaltkr/School_District_Analysis/blob/main/Images/scores_by_school_type_after_replace.png)
	
	After filtering out 9th grade ->
	![](https://github.com/Sheetaltkr/School_District_Analysis/blob/main/Images/scores_by_school_type_after_update.png)
		
		
## Summary

 The four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs are:

1. **District summary and School summary report are impacted** and show reduced values for Passing Math %, Passing Reading%, and Overall Passing %. 

2. **Top schools list on basis of Overall Passing % gets impacted** with **Thomas High School** losing its position from 2nd to 8th. Upon re-running the analysis this impact is 	no longer visible.

3. **Grade level Reading scores and Math scores % are impacted** for 9th grade in Thomas High School. They show "NAN" instead of numbers which makes the data useless.

4.  **School performance based on the budget per student, the school size and type of school is impacted** and show reduced values for Passing Math %, Passing Reading%, and Overall Passing %. Upon re-running the analysis this impact is no longer visible.
