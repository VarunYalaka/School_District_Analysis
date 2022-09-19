# School_District_Analysis

## Overview of Project
Maria, the chief data scientist for a city school district and responsible for analyzing information from a variety of sources and in a variety of formats. She has gotten an updated version of the student data with several changes. The date includes - 

* student_id 

* Student_name

* Grade

* School_name

* Reading_score

* Math_score

* School_type

* School_budget 

![Student_DF_Details](https://user-images.githubusercontent.com/44387918/190963333-59238498-fe77-4b13-a248-facd8d3c0684.png)


###  Analysis Deliverables:

1. Collect the student data into a DataFrame.

2. Prepare a cleaned version of the DataFrame.

3. Summarize key pieces of the data. 

4. Drill down into the data to analyze specific subsets.

5. Compare and contrast the data using grouping functions. 


### Analysis Results: 
1. Collect the student data into a DataFrame. 

* Imported the data using **_os.path.join()_** and created a student_df data frame. 

2. Prepare a cleaned version of the DataFrame.

* Checked and removed all rows with NaN, or missing, values in the student DataFrame. Drop rows using **_student_df = student_df.dropna()_** 

3. Summarize key pieces of the data. 

* Generated summary statistics using the **_describe_** function. i.e student_df.describe() 

4. Drill down into the data to analyze specific subsets.

* Analyzed reading and math scores by grades / school / school_type.  

5. Compare and contrast the data using grouping functions

* Compared district vs charter schools for budget and scores.

Detailed results are at the jupyter notebook link below: 
  
[Student_Data.ipynb](https://github.com/VarunYalaka/School_District_Analysis/blob/main/Student_Data_Starter_Code.ipynb)


## Conclusion

Interesting number of NaN values for reading and math-score. 

![NaN values count](https://user-images.githubusercontent.com/44387918/190964932-e1bdd6e7-3a23-4d5b-84b3-ee19ed0940c5.png)


We removed all the null value rows in this exercise. Maybe Average them is the best solution to mitigate. 

 
Based on the analysis Charter schools are producing higher scores with less budget. 

![Charter vs Public_school_Analysis](https://user-images.githubusercontent.com/44387918/190965005-1b179b03-7a6b-4be6-9eeb-4a94f491965d.png)


We removed the reading (1968) and math_scores (982) rows. Which is a higher number, these data may change the above result. Further, perform analysis based on the student count and grade helps to know the trends. 
