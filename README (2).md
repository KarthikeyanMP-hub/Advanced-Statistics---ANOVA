
# Advanced Statistics Project
## Problem Statement
### Problem 1A
### Salary is hypothesized to depend on educational qualification and occupation. To understand the dependency, the salaries of 40 individuals  are collected and each person’s educational qualification and occupation are noted. 
#### 1.State the null and the alternate hypothesis for conducting one-way ANOVA for both Education and Occupation individually.
#### 2.Perform a one-way ANOVA on Salary with respect to Education. State whether the null hypothesis is accepted or rejected based on the ANOVA results.
#### 3.Perform a one-way ANOVA on Salary with respect to Occupation. State whether the null hypothesis is accepted or rejected based on the ANOVA results.
### Problem 1B:
#### 1.What is the interaction between two treatments? Analyze the effects of one variable on the other (Education and Occupation) with the help of an interaction plot
#### 2.Perform a two-way ANOVA based on Salary with respect to both Education and Occupation (along with their interaction Education*Occupation).State the null and alternative hypotheses and state your results. How will you interpret this result?
#### 3.Explain the business implications of performing ANOVA for this particular case study.


## Problem 1
## Description of Dataset
The given dataset has details of 40 salaried individuals. 
Educational Qualification has three levels such as High school graduate, Bachelor, and Doctorate. Occupation is at four levels such as Administrative and clerical, Sales, Professional or specialty, and Executive or managerial.
### 1.EDA
### Dataset info
The dataset has 40 rows and 3 columns.The columns Education and Occupation are of object datatype.The Salary is of integer data type.There are no missing values in the dataset.
### 2.Descriptive Summary
Pandas describe() can provide a quick summary of the data set as outlined in the notebook.  The output of pandas describe(include="all") is shown below. Here, all columns of the DataFrame are included in the analysis.
From the summary stats we found  \
#### The salary range is found to be between 50103 to
260151. 
#### Out of 40 employees 16 employees have completed Doctorate and 13 out of 40 employees are working as Prof-speciality making them as most common education level and occupation level respectively of the dataset

### 3.Variable analysis
The distribution of the salary variable is  studied using Histogram & the Boxplot. 

### 4.ANOVA TEST
The ANOVA (Analysis of Variance) technique can be used when it is needed to compare more than two population means.This technique also establish the causation of why the means are behaving in a particular manner.There are two types of ANOVA such as OneWay Anova and Two-way Anova.

### 5.Hypothesis Framing & Testing 
#### Hypothesis of one-way ANOVA for Education
Let H0 be Null hypothesis & Ha be Alternate hypothesis
𝐻0: 𝜇1 = 𝜇2 = 𝜇3
𝐻𝑎: At least one Salary level is different from the rest.
Where
𝜇1, 𝜇2 , 𝜇3 represent the population mean salary of 3 different education levels such as
Bachelors, Doctorate & HS-grad.
#### Hypothesis of one-way ANOVA for Occupation
Let H0 be Null hypothesis & Ha be Alternate hypothesis
𝐻0: 𝜇1 = 𝜇2 = 𝜇3= 𝜇4
𝐻𝑎: At least one Salary level is different from the rest.
Where
𝜇1, 𝜇2 , 𝜇3, 𝜇4 represent the population mean salary of 4 different Occupation levels such as
Administrative and clerical, Sales, Professional or specialty, and Executive or managerial.

### One-way ANOVA on Salary w.r.t Education
#### Observation
##### The p value = 1.26e-08 which is less than the significance level (alpha = 0.05) 
#### Conclusion
we can reject the null hypothesis and conclude that atleast one Salary level is different from the rest based on education.

### One-way ANOVA on Salary w.r.t Occupation
#### Observation
##### The p value = 0.458508 which is greater than the significance level (alpha = 0.05)
#### Conclusion
we fail to reject the null hypothesis and conclude that there
is no significant difference in population mean salary of 4 different Occupation levels.

### Problem 1B
#### Interaction between two treatments
The interaction point plot is used to show the interaction between the categorical variables, Education and Occupation.

#### Two-way ANOVA based on Salary with respect to both Education and Occupation (along with their interaction Education*Occupation).
#### Null Hypothesis
𝐻0:There is no interaction effect between the 2 independent variables, education and occupation).
#### Alternate Hypothesis
𝐻1: There is an interaction effect between the variableS ‘education’ and ‘occupation’ on the mean Salary.

#### Observation:
The p value = 2.232500e-05 is lesser than the significance level (alpha = 0.05), we reject the null hypothesis.

#### Conclusion
##### There is a significant amount of interaction between the variables,Education and Occupation.
##### People with education as Doctorate draw the maximum salaries and people with education HS-grad earn the least. Thus, we can conclude that Salary is dependent on educational qualifications and occupation.
