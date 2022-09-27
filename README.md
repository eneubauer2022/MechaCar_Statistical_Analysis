# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG

![this is an image](https://github.com/eneubauer2022/MechaCar_Statistical_Analysis/blob/main/deliverable%201.png)

**- Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?**

  The p-values of both vehicle_length (2.60e-12) and ground_clearance (5.21e-08) were smaller than 0.05, so they would be considered variables that had a non-random amount of variance to the mpg values. Both variables would have a significant impact on mpg. 

**- Is the slope of the linear model considered to be zero? Why or why not?**

  No. the p-value is 5.35e-11 which is significantly lower than 0.05. The null hypthoesis must be rejected and that variables have an impact on mpg and are not random factors. 

**- Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?**

  Since we have a R-squared value of 0.71, we can determine that 71% of mpg is explained by the variables of our dataframame. I would feel comfortable using this model as as predictor of mpg for MechCar prototypes. 

## Summary Statistics on Suspension Coils

**The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?**

If we look at the total summary, it seems that maufacturing is meeting the design speficiations by keeps the the suspension coils under 100 pounds per inch.

![this is an image](https://github.com/eneubauer2022/MechaCar_Statistical_Analysis/blob/main/total%20summary.png)

However, once we breakdown those data points by manufacturing lots - we notice that Lot 3 has a high variance og 170.29, exceeding the 100 pounds per square inch specifications. Lots 1 & 2 fall under those weight specifications. 

![this is an image](https://github.com/eneubauer2022/MechaCar_Statistical_Analysis/blob/main/lot%20summary.png)
