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



## Summary Statistics on Suspension Coils

The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?


![total_summary](https://user-images.githubusercontent.com/104735724/183298741-59dadc2d-1b96-4d21-bd44-ed366065c186.PNG)

According to our results, the current manufacturing data meets this design specifications for all manufacturing lots in total. This shows that variance is 62.29 PSI, that is within requirements of not exceeding variance 100 PSI.


![lot_summary](https://user-images.githubusercontent.com/104735724/183298804-bb3a1b51-c5c9-497d-95db-7b9be93eeb7e.PNG)


The per-lot breakdown of the data shows Lot3 has a suspension coil variance of 170.2861224, which is above the variance limit of 100 pounds per square inch. Lot 1 (0.9897433) and Lot 2 (7.4693878) are within the variance limit and meet the design specification. 


## T-Tests on Suspension Coils

Findings: 


![t_test_one](https://user-images.githubusercontent.com/104735724/183299438-f7a7c30b-67f4-4c26-af3c-b9131824d336.PNG)

T-test for all lots vs. pop. mean of 1500 PSI - no statistical difference.


![t_test_two](https://user-images.githubusercontent.com/104735724/183299464-db7f2bc7-329d-40c7-aa1f-0b5716caaaf5.PNG)

T-test for lot 1 vs. pop. mean of 1500 PSI - no statistical difference.


![t_test_three](https://user-images.githubusercontent.com/104735724/183299526-7ce5d1b1-8fd9-47c5-b6ed-dd7b473246c7.PNG)

T-test for lot 2 vs. pop. mean of 1500 PSI - no statistical difference.


![t_test_four](https://user-images.githubusercontent.com/104735724/183299555-f8c98a40-7bb4-4e36-9430-f33949c1edb6.PNG)

 T-test for lot 3 vs. pop. mean of 1500 PSI - yes, a statistical difference.


## Study Design: MechaCar vs Competition


1. What metric or metrics will be tested?

- Overall Safety Rating: Safety Ratings are available at https://www.nhtsa.gov/ratings. The ‘overall’ category is made up of various sub-categories like: Frontal Crash, Side Crash, Rollover, etc.; but we just need a categorical ‘overall safety rating’ (e.g. A, B, C, D, E, and F).

- Vehicle Weight: We need the vehicle weight for all current cars. This can be converted into ‘buckets’ or categories. For example, for cars weighing 0.5 - 2.0 tons (e.g. 1000 - 4000 pounds), we would need twelve 250 pound weight ‘categories’.


2. What is the null hypothesis or alternative hypothesis?

- Null Hypothesis: The cars in the same class have the same fuel efficiencies.

- Alternative Hypothesis: Not all cars in the same class have the same fuel efficiences. 


3. What statistical test would will be used to test the hypothesis? And why?

- We would use ANOVA test. It would identify statistical difference between the distribution means from multiple samples.


4. What data is needed to run the statistical test?

- Model ID, Manufacturer, fuel efficiency data, class type data.

- It will need fuel efficiency data from 50 individual cars.

- Then we can create a sample size of data for each car in the class type. For example, if there were 10 cars in the class type, then we can have a top of 500 data points collected for each fuel efficiency type.


