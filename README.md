# Challenge 15 MechaCar Statistical Analysis

## Overview of the Project 
AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ upper management has called on the data analytics team to review the production data for insights that may help the manufacturing team.

[MechaCarChallenge.R](https://github.com/lfhoepers/MechaCar_Statistical_Analysis/blob/59a4ae57ff2866b4ff908718c7af498b82870666/MechaCarChallenge.R)

## Linear Regression to Predict MPG

![image](https://user-images.githubusercontent.com/100812079/172732472-a382cccd-a69d-4da8-ba4e-c60fdf06a85a.png)

The three takeaways addressing the three questions are as follows:

- Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
 
  the variance of a non-random variable is most of the time O, and provided this, the coefficients of the intercept, vehicle length and ground clearance can be said to give a non-random amount of variance to the MPG values.

- Is the slope of the linear model considered to be zero? Why or why not?
  
  The p-value for this model, 5.35e-11, is much smaller than the assumed significance level of 0.05%. This indicates there is sufficient evidence to reject the null hypothesis, and that the slop of this linear model would not be zero. 
  
- Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
  
  According to this regression model, the multiple R-squared of .71 shows there's a strong correlation but multiple R-aquared increases as more variables are passed through the regression. With an r-squared value this high, relatively speaking, this linear model does predict mpg of MechaCar prototypes effectively.
  

## Summary Statistics on Suspension Coils

![image](https://user-images.githubusercontent.com/100812079/172732775-c590713a-672f-4faa-8a2e-75aba9d56601.png)


![image](https://user-images.githubusercontent.com/100812079/172732756-b5191960-2b82-4b72-9905-287dcac0d85e.png)

The overall variance of all the lots indicates that the manufactoring data meets the design specification, having a variance of 62. However,  it is clear that variance in lot 3 is heavily increasing teh summary variance. Lo 3 has a variance of 170 PSI, meaning it does not pass the manufatcoring specifications. 1 and 2 are good.

## T-Tests on Suspension Coils

Performing a t-test on the suspension coil data, to determine whether there is a statistical difference between the mean of this provided sample dataset and a hypothesized potential population dataset, using a presumed population mean of 1500.

Across all manufacturing lots:

![image](https://user-images.githubusercontent.com/100812079/172733064-d3c9fb3a-25dc-4470-b523-82d94fa86798.png)

With a p-Value of 0.06, which is higher than the common significance level of 0.05, there is NOT enough evidence to support rejecting the null hypothesis.

However, if we look at t-test results for the three lots individually we find the following results:

For Lot 1:

![image](https://user-images.githubusercontent.com/100812079/172733092-bb5f4039-0b56-49b2-8753-6472a15491c0.png)

Measuring by a significance level of 0.05, we fail to reject the null hypothesis given the p-value equals 1. However, there is interesting correlation between the p-value and the confidence interval in that as the p-value increases, the confidence interval decreases - which can indicate there's more accuracy in precicting the true population mean

For Lot 2:

![image](https://user-images.githubusercontent.com/100812079/172733111-ab758f4c-4e2a-48f9-8b24-9803eada1854.png)

Measuring by a significance level of 0.05, we fail to reject the null hypothesis given the p-value equals .61. Again, the confidence interval is quite narrow with Lot 2 as well.

For Lot 3:

![image](https://user-images.githubusercontent.com/100812079/172733119-662b9f52-dcbe-4854-ae49-09033d2e51d3.png)

Measuring by a significance level of 0.05, we can reject the null hypothesis given the p-value equals .04. Additionally, the mean of the Lot 3 sample is also significantly smaller in comparison to the previous two lots. Especially important is that Lot 3 does not include the predicted population mean unlike the first two.


## Study Design: MechaCar vs Competition

I would like to see MechaCar conduct a statistical study on the depreciation of their vehicals similat to that of their competitors.

Metrics: Depreciation Rate over the life of the vehicle.

The null hypothesis would be there is no statistical difference between rate of depreciation for MechaCar and the competition.

The alternative hypothesis would be there is a statistical difference between rate of depreciation for MechaCar and the competition.

Statistical test: To complete this study, the analysts at MechaCar would want to use linear regression. as this would show you the depreciation over time.

Data: 
Age
Mileage
Condition
Make
Model


I appreciate the opportunity to present this project, I am available for any clarification.

**Luiz Fernando Hoepers**

**UofT SCS Data Analytics Boot Camp**
