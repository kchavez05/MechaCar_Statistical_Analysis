# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG
![img](https://github.com/kchavez05/MechaCar_Statistical_Analysis/blob/main/mpg_summary.PNG)
### Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
Ground clearance and vehicle length provide non-random variance to the mpg values in the dataset.

### Is the slope of the linear model considered to be zero? Why or why not?
The slope of the linear model is not considered to be zero.  The r-squared value is .6825 so there is a reasonably strong positive correlation in mpg with the given set of variables.

### Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
It does.  The p-value of the model is well below our desired significance level.  However, because only two of the six metrics have significant correlation with mpg, it may be worthwhile to modify the dataset by either including more data, or limiting the variables to those that are significant.

## Summary Statistics on Suspension Coils
![img](https://github.com/kchavez05/MechaCar_Statistical_Analysis/blob/main/total_summary.PNG)
![img](https://github.com/kchavez05/MechaCar_Statistical_Analysis/blob/main/lot_summary.PNG)
### The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?
The current manufacturing data as a whole meet the design specifications, as do Lot 1 and Lot 2 individually.  The variance in Lot 3 exceeds the design specifications.

## T-Tests On Suspension Coils
The t-tests comparing PSI across manufacturing lots show that each lot has approximately the same mean value - quite close to 1500 PSI - which is the same as the population mean.

## Study Design: MechaCar vs Competition
If one wanted to compare the MechaCar against cars made by competitors we could choose to look at a number of different metrics.  Some potentially useful comparisons could be price, city/highway fuel efficiency, engine performance, or even safety ratings.  For example, comparing price to engine performance could be useful to see how a customer could get the most "bang for their buck" as it were.  Or, for the environmentally conscious consumer, comparing price against fuel efficiency could be valuable to see if long-run gas savings could be worth spending more on a given vehicle.

The null hypothesis for any of these comparisons would be that price has no correlation to engine performance or fuel efficiency.  The alternative hypothesis would be the inverse - that engine performance or fuel efficiency is correlated (positively or negatively) to price.  It would be sensible to assume that, for example, a vehicle with higher horsepower would be more expensive.  However, a two-sample t-test would be able to tell us if, or how significant, the correlation is.

The data needed to test these hypothesis would be price of MechaCar and competing vehicles as well as data on mpg, horsepower, safety rating, etc.
