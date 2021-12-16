# MechaCar_Statistical_Analysis

## Overview of Project
AutosRUs' latest prototype the MechaCar, is suffering from production troubles that are blocking the manufacturing team's progress. AutosRUS' upper management has requested a review of the production data for insights that may help the manufacturing team. 
Markup : * Perform multiple linear regression analysis to identify which variables in the   dataset predict the mpg of MechaCar prototypes.
         * Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots
         * Run t-tests to determine if the manufacturing lots are statistically different from the mean population
         * Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. For each statistical analysis, you’ll write a summary interpretation of the findings. 

### Linear Regression to Predict MPG
The MechaCar dataset consists of 50 observations with 6 variables:
 
Markup : * vehicle_length
         * vehicle_weight
         * spoiler_angle
         * ground_clearance
         * AWD
         * MPG
         
 Markup : * Bullet list
              * Nested bullet
                  * Sub-nested bullet etc
          * Bullet list item 2

-OR-

 Markup : - Bullet list
              - Nested bullet
                  - Sub-nested bullet etc
          - Bullet list item 2 

## Statistical Summary
![Statistical Summary](https://github.com/john10roberts/MechaCar_Statistical_Analysis/blob/main/Resources/MechaMPGSummary.png)

Vehicle length and vehicle ground clearance provide a non-random amount of variance as indicated by having p values of less than .05. All other variables have p values larger than .05. The overall p value of the model is also less than .05 which shows that the slope of the line is not equal to zero. This model predicts the MPG of the mechacar effectively as it has an R-squared value of .7149 which using Pearson's Correlation value anything greater than .70 is considered a strong correlation. 

### Summary Statistics on Suspension Coils
The Suspension_Coil dataset consists of 150 observations with 3 variables:
 
Markup : * vehicleID
         * Manudacturing_Lot
         * PSI

## Statistical Summary
![Total Summary](https://github.com/john10roberts/MechaCar_Statistical_Analysis/blob/main/Resources/TotalSummary.png)

![Lot Summary](https://github.com/john10roberts/MechaCar_Statistical_Analysis/blob/main/Resources/LotSummary.png)

Overall, the variance for the suspension coils shows at 62.29 pounds per square inch which is very much within the design specifications that dictates that variance of the coils should not exceed 100 pounds per square inch. Additionally, lots 1 & 2 are well within the specifications. However, lot 3 is showing a variance of 170.29 pounds per square inch which is significantly outside of the specs. 

### T-Tests on Suspension Coils
Using your knowledge of R, perform t-tests to determine if all manufacturing lots and each lot individually are statistically different from the population mean of 1,500 pounds per square inch.

## Statistical Summary
![T-Test Total Summary](https://github.com/john10roberts/MechaCar_Statistical_Analysis/blob/main/Resources/TTestSummary.png)

The t-test across all the lots shows a p-value of .06028 which is higher than the .05 threshold this suggests that the means are similar statistically similar to the population mean of 1,500 pounds per square inch. 

![Lot1 T-Test Summary](https://github.com/john10roberts/MechaCar_Statistical_Analysis/blob/main/Resources/Lot1TTestSummary.png)

The t-test of Lot 1 shows a p-value of 1 which is higher than the .05 threshold and suggest that the means for the lot are statistically similar to the population mean of 1,500 pounds per square inch. 

![Lot2 T-Test Summary](https://github.com/john10roberts/MechaCar_Statistical_Analysis/blob/main/Resources/Lot2TTestSummary.png)

The t-test of Lot 1 shows a p-value of .61 which is higher than the .05 threshold and suggest that the means for the lot are statistically similar to the population mean of 1,500 pounds per square inch. 

![Lot3 T-Test Summary](https://github.com/john10roberts/MechaCar_Statistical_Analysis/blob/main/Resources/Lot3TTestSummary.png)

The t-test of Lot 1 shows a p-value of .04 which is less than the .05 threshold and suggest that the means for the lot are not statistically similar to the population mean of 1,500 pounds per square inch. 

### Study Design: MechaCar vs Competition
Write a short description of a statistical study that can quantify how the MechaCar performs against the competition. In your study design, think critically about what metrics would be of interest to a consumer: for a few examples, cost, city or highway fuel efficiency, horsepower, maintenance cost, or safety rating.

Price would be the study that I would like to quantify how MechaCar performs against its competition. I would begin by collecting data across all manufacturers for:

Markup : * Price
         * Cost of Ownership
         * MPG
         * Resale Value

The null hypothesis would be that the MechaCar is priced correctly based on the metrics provided. The alternative hypothesis would then be that MechaCare is not priced correctly based on the metrics provided. 

This would suggest using a multiple linear regression test to determine which factors have the biggest impact on price. At that point we should be able to provide data to either accept or reject the null hypothesis. 

