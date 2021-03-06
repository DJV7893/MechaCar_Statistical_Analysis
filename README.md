# MechaCar_Statistical_Analysis
---
## Overview
---
### Purpose:

A few weeks after starting his new role at AutoRUs, Jeremy is approached by upper management about a special project. AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ upper management has called on Jeremy and the Data Analytics team to review the production data for insights that may help the manufacturing team.

We will help Jeremy and the Data Analytics team do the following:

   1. Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes
   2. Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots
   3. Run t-tests to determine if the manufacturing lots are statistically different from the mean population
   4. Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. For each statistical         analysis, you’ll write a summary interpretation of the findings.

---
## Deliverable 1
---
### Linear Regression to Predict MPG

From our Linear Regression Model Summary Table below we can observe the following:

   1. Vehicle Length and Ground Clearance are statistically likely to provide non-random amounts of variance to the model. Which means that the                   Vehicle Length and Ground Clearance have a significant impact on miles per gallon on the MechaCar prototype. Furthermore Vehicle Weight,                   Spoiler Angle, and All Wheel Drive (AWD) have p-values that demonstrate a random amount of variance in the dataset.
   2. The p-value for our model, 5.35e-11, is notably smaller than the assumed significance level of 0.05%. This implies that there is sufficient                 evidence to reject our null hypothesis, which further proves that the slope of our linear model is not zero.
   3. The linear model has an r-squared value of 0.7149, which means that approximately 71% of all mpg predictions will be determined by this model.             Accordingly, our multiple regression model does predict mpg of MechaCar prototypes effectively.

      <img width="502" alt="Linear_Regression_Model_Summary" src="https://user-images.githubusercontent.com/99817571/171870705-290d54a6-1ea8-4d0f-b27b-29e6468664a2.png">

---
## Deliverable 2
---
### Summary Statistics on Suspension Coils

In our Total Summary Table below for all manufacturing lots, the variance of the suspension coils is 62.29 PSI, which is well within the 100 PSI          variance requirement. Moreover, if we seperate the manufacturing lot data by each seperate lot as shown in our Lot Summary table, we can observe that Lot 1 and Lot 2 are well within the 100 PSI variance requirement; with variances of 0.98 and 7.47 respectively. Lot 3 is pushing the variance up in the Summary Table with a variance of 170.29. It is Lot 3 that is signicantly impacting the variance at the total manufacturing lot level.

   1. Total Summary Table
      
      <img width="337" alt="Total_Summary" src="https://user-images.githubusercontent.com/99817571/171877133-f4538095-d257-4f30-a2bd-17d980faeb3d.png">  
   
   2. Lot Summary Table                                    

      <img width="491" alt="Lot_Summary" src="https://user-images.githubusercontent.com/99817571/171877208-072b9a1b-66a7-43cf-9e68-ccb2071ccaed.png">       
      
---
## Deliverable 3
---
### T-Tests on Suspension Coils

All Manufacturing Lots:
With a p-V\value of 0.06, which is higher than the standard significance level of 0.05, there is not enough evidence to reject the null hypothesis. Which means that the mean of all three of these manufacturing lots is statistically similar to the presumed population mean of 1500.

<img width="403" alt="Summary_t-test" src="https://user-images.githubusercontent.com/99817571/171884847-9c594d9b-823b-457c-97da-cf88c57c2c25.png">

Lot 1:
With a p-value of 1 we cannot reject the null hypothesis that there is no statistical difference between the observed sample mean and the presumed population mean (1500).

<img width="472" alt="Lot1_t-test" src="https://user-images.githubusercontent.com/99817571/171888622-9163c978-b089-4e02-867b-235429e712ea.png">

Lot 2:
With a p-Value of 0.61 we cannot reject the null hypothesis that there is no statistical difference between the observed sample mean and the presumed population mean (1500).

<img width="470" alt="Lot2_t-test" src="https://user-images.githubusercontent.com/99817571/171889675-613fcb48-13ca-4667-91af-df5bc43f03be.png">

Lot 3:
With a p-Value of 0.04, which is lower than the standard significance level of 0.05, we can reject the null hypothesis that this sample mean and the presumed population mean are not statistically different.

<img width="472" alt="Lot3_t-test" src="https://user-images.githubusercontent.com/99817571/171891222-cfb852e6-226e-4e1d-9f16-76ca8f235f0f.png">

---
## Deliverable 4
---
### Study Design: MechaCar vs Competition

For our additional statistical study to compare performance of the MechaCar vehicles against performance of vehicles from other manufacturers, we will collect data from various manufacturers comparable models over the last 5 years. We will collect data from these comparable models for the following metrics: 

   1. Dependent Variable: Current Price(Selling)
   2. Independet Variables: Safety Feature Rating (Independent Variable), MPG (Gasoline Efficiency), Resale Value

Our Null Hypothesis will be: MechaCar is priced correctly based on its performance in key factors for its model type.

Our Alternative Hypothesis will be: MechaCar is not priced correctly based on its performance in key factors for its model type.

To implement our study we will run a Multiple Linear Regression to determine the factors that have the highest correlation with the Current Price(Selling) and which independent variables has/have the greatest effect on Selling Price.

---
## Resources
---
Data Source: [MechaCar_mpg.csv](https://github.com/DJV7893/MechaCar_Statistical_Analysis/files/8834068/MechaCar_mpg.csv), [Suspension_Coil.csv](https://github.com/DJV7893/MechaCar_Statistical_Analysis/files/8834069/Suspension_Coil.csv)

Software: RStudio
