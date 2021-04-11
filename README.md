# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG
![MechaCar_1](Resources/MechaCar_1.png)

* Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset? 
    * According to our results, vehicle length and ground clearance are are statistically unlikely to provide random amounts of variance to the linear model, which indicates they have a greater impact on vehicle MPG.
* Is the slope of the linear model considered to be zero? Why or why not?
    * The slope of the linear model is not zero. The calculated p-value (5.35e-11) is much less than the assumed significance level of 0.05, which means there is sufficient evidence to reject the null hypothesis, meaning the slope of our linear model is not zero.
* Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
    * This multiple linear regression model has an r-squared value of 0.71 so, roughly 71% of MPG predictions of the MechaCar prototypes will be accurate when using this model.