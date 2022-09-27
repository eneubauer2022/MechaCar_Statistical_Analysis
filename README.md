# MechaCar_Statistical_Analysis

## Background

A few weeks after starting his new role, Jeremy is approached by upper management about a special project. AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ upper management has called on Jeremy and the data analytics team to review the production data for insights that may help the manufacturing team.

In this challenge, you’ll help Jeremy and the data analytics team do the following:

Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes
Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots
Run t-tests to determine if the manufacturing lots are statistically different from the mean population
Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. For each statistical analysis, you’ll write a summary interpretation of the findings.

- Deliverable 1: Linear Regression to Predict MPG
- Deliverable 2: Summary Statistics on Suspension Coils
- Deliverable 3: T-Test on Suspension Coils
- Deliverable 4: Design a Study Comparing the MechaCar to the Competition

## Linear Regression to Predict MPG

![this is an image](https://github.com/eneubauer2022/MechaCar_Statistical_Analysis/blob/main/deliverable%201.png)

**- Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?**

  The p-values of both vehicle_length (2.60e-12) and ground_clearance (5.21e-08) were smaller than 0.05, so they would be considered variables that had a non-random amount of variance to the mpg values. Both variables would have a significant impact on mpg. 

**- Is the slope of the linear model considered to be zero? Why or why not?**

  No. the p-value is 5.35e-11 which is significantly lower than 0.05. The null hypothesis must be rejected and that variables have an impact on mpg and are not random factors. 

**- Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?**

  Since we have a R-squared value of 0.71, we can determine that 71% of mpg is explained by the variables of our data frame. I would feel comfortable using this model as as predictor of mpg for MechCar prototypes. 

## Summary Statistics on Suspension Coils

**The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?**

If we look at the total summary, it seems that manufacturing is meeting the design specifications by keeps the suspension coils under 100 pounds per inch.

![this is an image](https://github.com/eneubauer2022/MechaCar_Statistical_Analysis/blob/main/total%20summary.png)

However, once we breakdown those data points by manufacturing lots - we notice that Lot 3 has a high variance of 170.29, exceeding the 100 pounds per square inch specifications. Lots 1 & 2 fall under those weight specifications. 

![this is an image](https://github.com/eneubauer2022/MechaCar_Statistical_Analysis/blob/main/lot%20summary.png)


## T-Tests on Suspension Coils

Using our knowledge of R, we performed the below T-Tests on all the lots and then each lot to see if there was any statistical difference. We used a mean of 1,500 for the mean. 

T-Test for All Lots. There was no statistical difference because the p-value was greater than 0.05.

![this is an image](https://github.com/eneubauer2022/MechaCar_Statistical_Analysis/blob/main/t.test.png)

T. Test of Lot 1. There was no statistical difference because the p-value was greater than 0.05.

![this is an image](https://github.com/eneubauer2022/MechaCar_Statistical_Analysis/blob/main/lot1.png)

T. Test of Lot 2. There was no statistical difference because the p-value was greater than 0.05.

![this is an image](https://github.com/eneubauer2022/MechaCar_Statistical_Analysis/blob/main/lot2.png)

T. Test of Lot 3. There was a statistical difference because the p-value was less than 0.05.

![this is an image](https://github.com/eneubauer2022/MechaCar_Statistical_Analysis/blob/main/lot3.png)

## Study Design: MechaCar vs Competition

**What metric or metrics are you going to test?**
  - Overall Safety rating. We will compare how the safety ratings of MechaCar's prototypes will compare against the competition. We will need to put each of the vehicles into a "category" bucket based on a letter grade to indicate their overall safety (A, B, C, D, etc.)
  - Vehicle maintenance. We will also compare how often a car is seen for maintenance. We can bucket these maintenance visits into time frames (monthly check-up, 3-month checkup, 6-month check-up, 1-year check-up, 2-year-checkup)
  - Vehicle resale value - we also want to understand if either of the above factors have an impact on the resale value of the vehicle when it is resold as a used card. 

**What is the null hypothesis or alternative hypothesis?**

Null Hypothesis: Safety ratings and regular vehicle maintenance have no impact on resale value. 

Alternative Hypothesis: A higher safety rating and monthly vehicle maintenance can increase the resale value of a car by almost 50%. 


**What statistical test would you use to test the hypothesis? And why?**

Chi-squared Test - "Is there a difference in categorical frequencies between groups?"

**What data is needed to run the statistical test?**

- We will need to know the safety ratings of each of the vehicles for MechaCar and their competitors.

- We will need to know how often vehicles are taken in for regular maintenance and the time frame from the last time they received maintenance. 

- We will need to know how much the vehicle was resold for.
