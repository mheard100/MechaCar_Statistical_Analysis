# MechaCar_Statistical_Analysis

## Project Overview
In this project, statistics and hypothesis testing is used to analyze datasets from the automotive industry with R Studio and R programming language.

## Tools and Techniques 
R-programming, dyplr, tidyverse, ggpot2, Statistical Tests, Hypothesis Testing, A/B Testing 

## Linear Regression to Predict MPG

![Linear Regression Summary](https://github.com/mheard100/MechaCar_Statistical_Analysis/blob/main/Linear%20Regression%20Summary.PNG)
Interprepation of the multiple linear regression results: 
- Vehicle length, ground clearance and intercept have provided a non-random amount of variance to mpg values in the dataset. The intercept is statistically significant meaning there are other variables that do contribute to mpg that have not been included in the model. Spoiler angle, AWD and Vehicle weight contribute a random amount of variance to this linear model. 
- With an assumed significance level of 0.05%, the p-value of this linear model is 5.35e-11 which is much smaller than our significance level. Thus, we do not have enough evidence to reject the null hypothesis and the slope of the linear model is not zero. 
- In this linear model the r-squared value is an effective 0.7149 which means approximately 71% of all the mpg predictions will be correct when using this model.  

## Summary Statistics on Suspension Coils 

![total summary](https://github.com/mheard100/MechaCar_Statistical_Analysis/blob/main/total_summary.PNG)

The specifications for the design of MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per inch. According to the total summary, the variance is approximately 62 pounds per inch which is below the mandated value and meets design specification. 


![Lot summary](https://github.com/mheard100/MechaCar_Statistical_Analysis/blob/main/Lot_summary.PNG)

 From the above data we can see that the variance for Lot 1 and Lot 2 are 0.98 and 7.47 respectively. The current manufacturing data for Lot 1 and Lot 2 meet this design specification. However, the variance for Lot 3 is around 170 which is above the design specifications and does not meet the requirement. 

## T-Tests on Suspension Coils 

t-test that compares all manufacturing lots against mean PSI of the population:

Assuming a significance level of 0.05 percent, p-value (0.06028) is above our significance level. Therefore, we do not have enough evidence to support to reject the null hypothesis, and the two means are statistically similar. 


Suspension Coil lots:

Assuming a significance level of 0.05, p-value (1) is above our significance level for lot 1. Lot 2's p-value of 0.6072 is also above our significance level. We do not have enough evidence to support or reject the null hypothesis, and say the two means are statistically similar. 


Assuming a significance level of 0.05, p-value (0.04168) is below our significance level for lot 3. Therefore, we have enough evidence to reject the null hypothesis, and we would state that the two means are statistically different. 


## Study Design: MechaCar vs Competition 

Statistical Analysis of Cost
Cost is a big factor for people buying cars because customers need to stay in their price range. The study would answer if the cost of MechaCars is less than the competition. The Null hypothesis would be the means of cost for all cars across MechaCar and the competition are equal and the alternate hypothesis would be at least one of the means is different from all other groups. An ANOVA test would be useful for this because it is used to compare the means of a continuous numerical variable across a number of groups.A two-way Anova test would be useful for fuel mileage and model type since both are significant cost components. 
