# School District Analysis
Python pandas program for school district analysis

## Overview of the School district analysis

### Purpose

1. Help **Maria**, the chief data scientist for city school district present useful insights to **District School Board** and **Superintendent** by analyzing below **performance metrics** using clean **school funding** and **student test scores** data. This will help the key stakeholders in making decision regarding the district and school budgets and priorities.
2. Follow **Family Educational Rights and Privacy Act (FERPA)** and treat the data with utmost confidentiality to protect the students while working on school district analysis.
2. Re-analyze the data after disregarding **9th grade** Math and Reading scores for **Thomas high school** due to handle suspected Academic dishonesty
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



## Results

 - **How is the district summary affected?**
	
	Average Math Score, Passing Math %, Passing Reading%, and Overall Passing %  **decreased** by **0.1%,0.2%,0.3% and 0.1%** respectively. Average Reading Score was not impacted.
	
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
	**After replacing 9th grade math and reading scores with "NaN" values and considering the 9th grade student** count for calculating the Overall Passing % ; Thomas High School loses its position in Top 5 schools with **65%**
		![](https://github.com/Sheetaltkr/School_District_Analysis/blob/main/Images/Top_5_schools_after_replace.png)
	**After re-calculating the Overall Passing % with 9th grade student count removed;** Thomas High School recovers its second position in Top 5 schools with **90.6%**
		![](https://github.com/Sheetaltkr/School_District_Analysis/blob/main/Images/Top_5_schools_after_update.png)

- **How does replacing the ninth-grade scores affect the following:**
	- Math and reading scores by grade 


		-  Math scores for 9th grade changed from 83.6% to NaN for Thomas High School
		
	  Before-> 
    ![](https://github.com/Sheetaltkr/School_District_Analysis/blob/main/Images/math_scores_by_grade_before.png)
	  After-> 
    ![](https://github.com/Sheetaltkr/School_District_Analysis/blob/main/Images/math_scores_by_grade_after.png)

      -  Reading scores for 9th grade changed from 83.7% to NaN for Thomas High School

	Before-> 
![](https://github.com/Sheetaltkr/School_District_Analysis/blob/main/Images/reading_scores_by_grade_before.png)	
	After-> 
![](https://github.com/Sheetaltkr/School_District_Analysis/blob/main/Images/reading_scores_by_grade_after.png)

	- Scores by school spending
	
	- Scores by school size
	- Scores by school type

## Summary

 Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.

1. 

2. THS moved from 2nd top passing% to 8th position

3.

4.

-----

##Deliverable 3 Requirements
Structure, Organization, and Formatting (7 points)
The written analysis has the following structure, organization, and formatting:

There is a title, and there are multiple sections (2 pt).
Each section has a heading and subheading (3 pt).
Links to images are working, and code is formatted and displayed correctly (2 pt).
Analysis (18 points)
The written analysis has the following:

Overview of the school district analysis:

The purpose of this analysis is well defined (3 pt).
Results:

There is a bulleted list that addresses how each of the seven school district metrics was affected by the changes in the data (10 pt).
Summary:

There is a statement summarizing four changes to the school district analysis after reading and math scores have been replaced (5 pt).
