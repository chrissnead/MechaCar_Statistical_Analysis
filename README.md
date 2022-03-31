# MechaCar_Statistical_Analysis

## Overview
This analysis looks at production data for an auto company. The findings below provide insight into the manufacturing issues the team is experiencing and clarifies how they can be resolved.

## Linear Regression to Predict MPG
- The vehicle_length and ground_clearance data provided a non-random amount of variance to the mpg values in the dataset. As seen in the below image, the p-values of 2.6x10<sup>-12</sup> and 5.21x10<sup>-8</sup> are not significant.

![linear regression model](Images/linear_regression_model.png)

- The slope is not considered to be zero as the p-value is 5.35x10<sup>-11</sup>. Because of this, there is sufficient evidence to reject the null hypothesis.

- With the r-squared value at 0.7149 or 71.5%, the accuracy of the linear model's predicttion of mpg for MechaCar prototypes is fair, but should be improved.

## Summary Statistics on Suspension Coils
The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. The current manufacturing data seems to meet this design specification in the total summary (first image below) but it can be seen when broken down by each lot in the lot summary (second image below), Lot3 goes well beyond the maximum 100 pounds per square inch at a variance of 170.29.

![total_summary](Images/total_summary.png)
![lot_summary](Images/lot_summary.png)

## T-Tests on Suspension Coils
Each t-test shares a fairly similar mean of x of around 1500. The discrepancy is in Lot3 where the p-value is less than 0.05, therefore should be rejected as null.

![t-test](Images/t-test.png)
![t-test Lot1](Images/t-test-Lot1.png)
![t-test Lot2](Images/t-test-Lot2.png)
![t-test Lot3](Images/t-test-Lot3.png)

## Study Design: MechaCar vs Competition
To further measure MechaCar against competitors, the first metric I would look at is highway fuel efficiency. With vehicles increasingly becoming more powerful and full electric cars now being introduced to the market, fuel efficiency is a key metric in purchasing a vehicle. To test this, a linear regression model would be needed to understand outliers when measuring the MPG and horsepower for each vehicle.
