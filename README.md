# MechaCar-Analysis

## OVERVIEW OF PROJECT
The purpose of this project is to analyze AutosRUs' newest prototype, the MechaCar, which is suffering from production issues that affect the manufacturing team's progress. We also dive into the different metrics that affect its production and compare vehicle perfomance across different manufacturing lots. These metrics include vehicle length, weight, spoiler angle, ground clearance, AWD capabilities, MPG and PSI. 

## LINEAR REGRESSION TO PREDICT MPG


![Deliverable_One_LM](https://user-images.githubusercontent.com/104735724/183298381-6ef232e6-eee4-42b8-9009-b3477ad82922.PNG)


1. Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
According to our results, vehicle length with p-value=2.60e-12 which is « 0.05 and ground clearance with p-value=2.60e-12 which is « 0.05 provided a non-random amount of variance to the mpg values in the dataset having the most significant impact. 

2. Is the slope of the linear model considered to be zero? Why or why not?
No. The p-value is 5.35 x 10-11 which is much lower than our assumed significance level of 0.05%. That indicates that our slope of our linear model is not zero, and there is significant linear relationship between variables and mpg of the MechaCar prototype. 

3. Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
Yes. The r-squared is 0.7149 and indicates a strong positive linear relationship. This means that this model will have a 71.49% effective rate of predicting the mpg of MechaCar prototypes. 
