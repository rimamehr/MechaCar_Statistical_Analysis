# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG 

**- Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?**

  As seen in our output image below Vehicle weight, spoiler_angle & AWD provided a non-random amount of variance to the mpg value. In other words these variables have a
  significant impact on mpg value. The two variables that had the most amount of random variance to our mpg values are ground_clearance and vehicle_length.
    
    
**- Is the slope of the linear model considered to be zero? Why or why not?**

  Our P-value is 5.35e-11 which is lower than the alpha value of 0.05 which suggests that the slope is not zero, which in turn suggests that changes in the predictor variable are 
  associated with changes in the response variable.
  
  
**- Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?**

  Our R-squared value is what predicts the effectiveness of our model. R-squared is always between 0 and 100%. With a R-squared value of 0.7149 in our analysis below can predict
  the mpg of MechaCar protypes effectively about 71.49%. This means, there are other variables and factors that contribute to the variation in mpg that have not been included in
  our model. These variables may or may not be within our dataset and may still need to be collected or observed.
  
  <p align="left">
  <img src="/Images/Deliverable_1_output.png" width="500">
  </p>


## Summary Statistics on Suspension Coils

**- The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current
  manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?**
  
  Our mean PSI value for all manufacturing lots from the total_summary table is 1498.78 with a variance of 62.29 which is within the 100 PSI as per the design specifications. When
  we look at each lot individually in our lot_summary table, we notice that the lot1 and lot2 meet the design specification but the lot3 has a variance of 170.286 which is higher 
  than the acceptable limit.
  
  


<p align="left">                                                  <p align="right">                                                         
  <img src="/Images/total_summary.png" width="500">                   <img src="/Images/lot_summary.png" width="500">
  </p>                                                                </p>
  
  
  
  
  
  # All lots T-test                                                 # Lot1 T-test
  <p align="left">                                                  <p align="right">                                                         
  <img src="/Images/ttest_all.png" width="500">                   <img src="/Images/ttest_lot1.png" width="500">
  </p>                                                                </p>
  
  # Lot2 T-test                                                     # Lot3 T-test
  <p align="left">                                                  <p align="right">                                                         
  <img src="/Images/ttest_lot2.png" width="500">                   <img src="/Images/ttest_lot3.png" width="500">
  </p>                                                                </p>
  
  
