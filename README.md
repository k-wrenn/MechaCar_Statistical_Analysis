# MechaCar_Statistical_Analysis

## Project Overview
AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ upper management has called for a review of the production data for insights that may help the manufacturing team.

A multiple linear regression analysis was performed to identify which variables in the dataset predict the MPG of MechaCar prototypes. Summary statistics were collected on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots. Lastly, T-tests were run to determine if the manufacturing lots are statistically different form the mean population.

## Resources
Software: R, Rstudio

Data: MechaCar_mpg.csv, Suspension_Coil.csv

## Linear Regression to Predict MPG
![MechaCar_1](https://github.com/k-wrenn/MechaCar_Statistical_Analysis/blob/main/Resources/MechaCar_1.PNG)

* Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset? 
    * According to our results, vehicle length and ground clearance are are statistically unlikely to provide random amounts of variance to the linear model, which indicates they have a greater impact on vehicle MPG.
* Is the slope of the linear model considered to be zero? Why or why not?
    * The slope of the linear model is not zero. The calculated p-value (5.35e-11) is much less than the assumed significance level of 0.05, which means there is sufficient evidence to reject the null hypothesis, meaning the slope of our linear model is not zero.
* Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
    * This multiple linear regression model has an r-squared value of 0.71 so, roughly 71% of MPG predictions of the MechaCar prototypes will be accurate when using this model.


## Summary Statistics on Suspension Coils
The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch.

When looking at all the lots together, it appears the suspension coils are within the design specifications because the variance is 62.29 PSI, which is below the 100 PSI design specifications.

![Total_summary](https://github.com/k-wrenn/MechaCar_Statistical_Analysis/blob/main/Resources/Total_summary.PNG)

However, when we examine each lot individually, we can see the variance of Lot 3 does not sit below the 100 PSI threshold set forth by the design specificatoins.

![Lot_summary](https://github.com/k-wrenn/MechaCar_Statistical_Analysis/blob/main/Resources/Lot_summary.PNG)

Lot 1 and Lot 2 still meet the design specifications for MechaCar suspension coils with variances of 0.98 and 7.47 PSI per square inch, respectively.

## T-Tests on Suspension Coils
T-tests were performed to determine if all manufacturing lots and each lot individually are statistically different from the population mean of 1,500 pounds per square inch.

![t_tests](https://github.com/k-wrenn/MechaCar_Statistical_Analysis/blob/main/Resources/t_tests.PNG)

Assuming a significance level 0f 0.05 percent, when looking at all manufacturing lots, our p-value (0.06) is above the significance level. Therefore we do not have sufficient evidence to reject the null hypothesis, and we would state the two means are statistically similar.

Still assuming a 0.05 significance level, we examined each lot individually. Lot 1 provided a p-value of 1, lot 2 had a p-value of 0.61, and lot 3 had one of 0.04. Lots 1 and 2 provide p-values greater than the significance level which, again, means there is not sufficent evidence to reject the null hypothesis and the means are statistically similar. Lot 3, however, has a p-value less than the significance level, indicating lot 3 does have sufficient evidence to reject the null hypothesis, which means the two means are not statistically similar. 

## Study Design: MechaCar vs. Competition
Now that MechaCar has collected some data on its prototype vehicle, they may want to compare their data to that of current competitors. 

I would suggest looking at MPG, both city and highway, and comfort level. Many consumers are looking for a comfortable ride with high MPG.

The null hypothesis for this analysis would be the mean values for all vehicles (MechaCar and competitors) is the same. The alternative hypothesis would be that there is a statistically significant difference in at least one of the means.

An ANOVA test would be beneficial for this analysis because we are examining at data from multiple samples, as we would be comparing MechaCar to multiple different manufacturers.

In order to conduct the ANOVA test we would need to make sure the dependent variables (MPG and comfort) are numerical and continuous and the independent variable (manufacturer) is categorical. Before conducting the test, we need to make sure the dependent variable is considered to be normally distributed and the variance among each group is similar. We would also need a reasonably large sample size to increase the strength of the analysis. 
