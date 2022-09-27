# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG

Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

The p-values of both vehicle_length (2.60e-12) and ground_clearance (5.21e-08) were smaller than 0.05, so they would be considered variables that had a non-random amount of variance to the mpg values. Both variables would have a significant impact on mpg. 

Is the slope of the linear model considered to be zero? Why or why not?

No. the p-value is 5.35e-11 which is significantly lower than 0.05. The null hypthoesis must be rejected and that variables have an impact on mpg and are not random factors. 

Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

Since we have a R-squared value of 0.71, we can determine that 71% of mpg is explained by the variables of our dataframame. I would feel comfortable using this model as as predictor of mpg for MechCar prototypes. 
