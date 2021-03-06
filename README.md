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
  
 <p float="left">
  <img src="/Images/total_summary.png" width="500" />
  <img src="/Images/lot_summary.png" width="500" /> 
</p> 
  
  
 ## T-Tests on Suspension Coils
 
 **- Summary of interpretation and findings for the t-test results**
 
  -- Below are the t-tests for overall and **all three lots** individually. From the output, the p-value for lot1 is greater than the significance level 0.05 implying that the
      distribution of the data is not significantly different from normal distribtion. In other words, we can assume the normality.
      
       # All lots T-test                                                
  <p align="left">                                                                                                 
  <img src="/Images/ttest_all.png" width="500">                   
  </p>    
 
  -- From the output, the p-value for **lot1** is also greater than the significance level 0.05 implying that the distribution of the data is not significantly different from
      normal distribtion. In other words, we can assume the normality.
      
       # Lot1 T-test
  <p align="left">
   <img src="/Images/ttest_lot1.png" width="500">
 
  -- From the output, the p-value for **lot2** is greater than the significance level 0.05 implying that the
     distribution of the data are not significantly different from normal distribtion. In other words, we can assume the normality.
     
     # Lot2 T-test                                                     
  <p align="left">                                                                                                          
  <img src="/Images/ttest_lot2.png" width="500">                   
  </p> 
 
  -- From the output, the p-value for **lot3** is less than the significance level 0.05 implying that the
     distribution of the data is significantly different from normal distribtion. In other words, we cannot assume the normality.
     
      # Lot3 T-test
  <p align="left"> 
  <img src="/Images/ttest_lot3.png" width="500">
  </p>
     
  **-- So we can conclude from our overall results and the one for lot1 and lot2, the data is considered to have normal distribution.Therefore, we do not have sufficient evidence
  to
     reject the null hypothesis, and we would state that the two means are statistically similar.**

  
  ## Study Design: MechaCar vs Competition

Here, we are comparing how the MechaCar performs against its competition. There are certain metrics that would be of interest to a consumer like cost, city or highway fuel
efficiency, horse power, maintenance cost, safety rating, color (The most popular color, according to data provided by iSeeCars.com, is white, followed closely by black. Then
gray, then silver). In order to do this we want to answer four different questions which are:

### What metric or metrics are you going to test? ###
The metric that I would like to test is cost. I would be interested in analyzing how competitively does MechaCar price its car by various categories in comparison to their
competitors.
### What is the null hypothesis or alternative hypothesis? ###
The null hypothesis is that the researcher's prediction is not true. In this case we would predict that MechaCar has its car similarly priced to its competitors. The alternative
hypothesis is that the researcher's predicted difference is true.

### What statistical test would you use to test the hypothesis? And why? ###
In this case we could perform a sample t-test which will give us a way to decide between a null hypothesis and an alternative hypothesis.
 
### What data is needed to run the statistical test? ###
We would take a sample data with certain features between MechaCar and its competitors to perform a t-test. From the output, we could compare the the p-value for Mechacar and its
competitors to see if it is greater than the significance level 0.05 implying that the distribution of the data is not significantly different from normal distribtion. In other
words, we can assume the normality and the fact that Mechacar has its vehicle priced similar to its competition. 
