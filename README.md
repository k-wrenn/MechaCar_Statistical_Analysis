# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG
![MechaCar_1](Resources/MechaCar_1.png)

* Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset? 
    * According to our results, vehicle length and ground clearance are are statistically unlikely to provide random amounts of variance to the linear model, which indicates they have a greater impact on vehicle MPG.
* Is the slope of the linear model considered to be zero? Why or why not?
    * The slope of the linear model is not zero. The calculated p-value (5.35e-11) is much less than the assumed significance level of 0.05, which means there is sufficient evidence to reject the null hypothesis, meaning the slope of our linear model is not zero.
* Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
    * This multiple linear regression model has an r-squared value of 0.71 so, roughly 71% of MPG predictions of the MechaCar prototypes will be accurate when using this model.


## Summary Statistics on Suspension Coils
The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch.

When looking at all the lots together, it appears the suspension coils are within the design specifications because the variance is 62.29 PSI, which is below the 100 PSI design specifications.

![Total_summary](Resources/Total_summary.png)

However, when we examine each lot individually, we can see the variance of Lot 3 does not sit below the 100 PSI threshold set forth by the design specificatoins.

![Lot_summary](Resources/Lot_summary.png)

Lot 1 and Lot 2 still meet the design specifications for MechaCar suspension coils with variances of 0.98 and 7.47 PSI per square inch, respectively.