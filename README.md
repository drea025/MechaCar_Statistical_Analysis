# MechaCar_Statistical_Analysis

## Overview
The purpose of this project is to analyze data that can aid in predicting the mpg of MechaCar prototypes, therefore we take a look at the data collected which is the summary statistics on the PSI of the suspension coils from the manufacuring lots and run some t-tests in order to properly desgn a statistical study to compare vehicle performance of the MechaCars and other vehicles.

## Linear Regression to Predict MPG
<img width="505" alt="Screen Shot 2022-06-26 at 8 37 19 PM" src="https://user-images.githubusercontent.com/100797549/175855444-6f8eebb9-9971-41a1-a6e2-eb30b4eca2af.png">

The MechaCar dataset has a sample size of 50 prototypes measuring the miles per gallon. The linear regression was calcualted using R in RStudio, looking at the facts we know that the variance of a non- random variable lies at about zerp, the intercept, vehicle_length and ground clearance are closer to this value which can equate to being a non-random amount of variance to the mpg values. Also while taking a look at the p-value and having a significance level of 95% we see that the mpg is greater than 0.05 as well the two other variables. The vehicle length and the ground clearance which determines that this data represents non-random amounts of variance as applied to the mpg values. 

While looking at the linear regression model we also noted that all of the slopes of the variables are fairly close to zero however they do not equal zero, which results in a non-zero slope.
Since this linear model had a r-squared slope of 0.71 we can assume that more than half of all mpg predictins will be determined by this model. And although that is a high percentage, it is not 100% accruate that it can predict mpgs of MechaCar prototypes effectively. 

## Summary Statistics on Suspension Coils
<img width="305" alt="Screen Shot 2022-06-26 at 8 55 39 PM" src="https://user-images.githubusercontent.com/100797549/175856992-028e4d5e-03ea-4bee-8d42-db8744054a51.png">
<img width="442" alt="Screen Shot 2022-06-26 at 8 56 21 PM" src="https://user-images.githubusercontent.com/100797549/175859006-763266ae-4dbc-4019-8d43-7abe24decf74.png">

The Suspension Coil dataset provided for the MechaCar contains the results of testing the weight capacities of multiple suspension coils from multiple production lots to determine consistency.By looking at the entire population of the production lot, the variance of the coils is 62.29 PSI, which is within the 100 PSI variance requirement.In total, the manufacturing data meets the maximum variance in PSI requirement, but we can see that there are clearly big problems in lot 3 with a variance of 170 PSI. Lot 3 does not meet the maximum variance requirement.

## T-Test on Suspension Coils
<img width="425" alt="Screen Shot 2022-06-26 at 9 00 47 PM" src="https://user-images.githubusercontent.com/100797549/175857434-5cc7151a-e39c-4fe3-80bd-a2e25cc48435.png">
By looking at the sample t-test we can see the true mean of the sample is 1498.78, which we also saw in the summary statistics above. With a p-Value of 0.06, which is higher than the common significance level of 0.05, so we can determine there isn't enough evidence to support rejecting the null hypothesis. That is to say, the mean of all three of these manufacturing lots is statistically similar to the presumed population mean of 1500. We can see that in lot 1 it does have the true sample mean of 1500 and a p-value of 1 so we will not reject the null hypothesis. Lot 2 has a very similar outcome to lot 1 therefore the conclusion will be equavalent to the previous, however lot 3 the sample mean came to 1496.14 and the p-value was below 1 therfore we reject the null hypothesis and the presumed population mean are not statistically different. We may conclude somthing went astray with this information and the quality of car should be checked in this lot.

## Study Design: MechaCar vs. Competition
Another statistical study that can be performed to determine MechaCar's standing against its competition is a linear regression on city and highway fuel efficiency. Gasoline is expensive nowadays, and it is an important feature that many consumers look at when purchasing a new car. In order to compare the performance of the MechaCar against the competition, we need to address a few observables which would be of interest to our customers. These variables will be cost, city and highway fuel efficiency, horsepower, safety rating, and carbon waste output. In order to run these statistical tests, we would need the cost, fuel efficiency, horsepower, safety rating, and carbon waste output data from the MechaCar as well as the MechaCar's competitors. Using a multiple linear regression statistical summary and a random sample of n > 30 for MechaCar we would see how the variables impact the safety ratings for MechaCar and their competitors.
