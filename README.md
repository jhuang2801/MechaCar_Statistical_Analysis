# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG

![Linear Regression](https://github.com/jhuang2801/MechaCar_Statistical_Analysis/blob/main/images/Linear%20Regression.png)

Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

- Vehicle length and ground clearance both have Pr(>|t|) (p-values) lower than 0.05, which means that they both have statistically significant relationsip to the response variable (mpg) to the model.

Is the slope of the linear model considered to be zero? Why or why not?

- The null hypothesis states that the slope is equal to zero, and the alternative hypothesis states that the slope is not equal to zero. The p-value of 5.35e-11 is lower than the significance value of 0.05, which means that it is sufficient to reject the null hypothesis, and the slope of the linear model is not considered to be zero. 

Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

- Since the multiple R square value is 0.7149 and the R adjusted value is 0.6825, the R values show a high level of correlation. 

## Summary Statistics on Suspension Coils

The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

![Total summary](https://github.com/jhuang2801/MechaCar_Statistical_Analysis/blob/main/images/total-summary.PNG)

![Lot summary](https://github.com/jhuang2801/MechaCar_Statistical_Analysis/blob/main/images/lot-summary.PNG)

- The variance of 100 pounds per square inch means it is no more than 100 psi. The design specs are respected for all manufacturing lots in total with a global variance of 62.3 psi. On the lot level, Lot 1 and Lot 2 are into specs (Lot 1 has variance of 0.98 psi and Lot 2 has variance of 7.5 psi). The Lot 3 is out of specs with a variance of 170.3 psi, which is greater than the acceptance limit of 100 psi.

## T-Tests on Suspension Coils

![Sample T Test](https://github.com/jhuang2801/MechaCar_Statistical_Analysis/blob/main/images/Sample-T-test.PNG)
![Lot T Test](https://github.com/jhuang2801/MechaCar_Statistical_Analysis/blob/main/images/Lot-T-Test.PNG)

- The p-value of 0.06028 is greater than the significance level at 0.05%, so it is not enough to reject the null hypothesis. Lot 1 has p-value at 1, which means it has the true sample mean of 1500 (no statistical difference). Lot 2's p-value is at 0.61 and the sample mean is 1500.02, which means that the null hypothesis cannot be rejected. Lastly, Lot 3 has p-value lower than 0.05 and the sample mean at 1496.14, which means we can reject the null hypothesis.

## Study Design: MechaCar vs Competition

The metrics we can test on MechaCar vs competiton can be set as price of the car vs its fuel efficiency (miles per gallon).

Null Hypothesis: MechaCar is cheap and fuel efficient.
Alternative Hypothesis: MechaCar is neither cheap nor fuel efficient.

To test the hypothesis, we can correlate the cost of MechaCar to see if it has a linear correlation to its fuel efficiency (miles per gallon), which means cost is directly proportional to fuel efficiency. To run statistical test, we would need to collect data on the mean, standard deviation, and variance on each model with cost and fuel efficiency. 
