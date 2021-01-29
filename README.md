## Moringa-DSC7-Week-4-IP
### Overview 
Just like before, we have been tasked to understand electric car usage by solving for another research question. We will work as a Data Scientist for the Autolib electric car-sharing service company to investigate a claim about the blue cars from the provided Autolib dataset.

In an effort to do this, we need to identify some areas and periods of interest via sampling stating the reason to the choice of method, then perform hypothesis testing with regards to the claim that we will have made. An example of claim to test would be "Is the number of Bluecars taken in area X different than in area Y? Is it greater in area X than in area Z? Etc”. The selected periods of interest be either weekdays or weekends but not a mix of both. You can also consider postal codes 75015 vs 75017 to some of the areas of interest. 

### To work on this project, we will perform the following analysis with Python; 

#### Find and deal with outliers, anomalies, and missing data within the dataset.
> Plot appropriate univariate and bivariate summaries recording our observations.
> Implement the solution by performing hypothesis testing.
> This will need to be documented when writing the report. 
##	Data Analysis
### Hypothesis testing results 
Before we begun our analysis, we tested the normality of our hypothesis to determine which test statistics to use in our analysis. After testing our normality, the data was normally distributed, therefore together with the other assumptions we used the t test. We used the Shapiro- Wilk test and (QQ)Plot to determine the normality. 
 After working on our t test, the test statistics is -0.102, which helps us make decision on either accepting or rejecting the null hypothesis. 
For the p-value, we found a value of 0.92 which will determine whether to reject or accept the null hypothesis. 

To find our point estimator, we find the mean of the overall number of the Blue Cars that were taken which is 49 and the mean of the sample taken from the blue cars taken to make parameter on the population which is 43. Therefore, finding our point estimate we find the difference of the means, the difference of the means is 6.
For the confidence interval, the lower bound and upper bound, these is meant to provide a range within which our means should lie under, our 33 lower bound 43 upper bound 52. Our sample mean 43 and population mean 49 lies within the set bound. 

#### Discussion of Test Sensitivity
Interval estimation aims at estimating a population parameter by specifying a range of values with lower limits and upper limits. The true value of the population parameter is believed to lie within these limits. Therefore, from our interval estimate population parameter lies within the range. It signifies our interval estimate. Since our sample size it was small, there was an error in our point estimate, a point estimate can never be perfect since its based on a sample but not the entire population thus resulting to an error. that’s forms the difference in the population mean and sample mean.
## Summary and Conclusion
We carried out different analysis on the data. A random sample was taken into account to avoid biasness in the data selected, sorting and filtering was taken into account to select certain variables and dataset. The outliers were eliminated to that we could work with data that ranged within the set limits. We did reset the index to determine the number of datasets. Correlation was taken into account to determine any relationships within and between the dataset, plots were created for visualization the correlation. There were no missing values in the dataset.
From our hypothesis we can conclude that, based on the p-value = 0.92 > α = 0.05, we fail to reject our null hypothesis. The difference between BlueCars taken sum and BlueCars returned sum of n daily data point of 1439 are not statistically significant. There was no enough evidence to show there was a difference in BlueCars taken and those returned. We therefore conclude that there was a relationship between the blue cars that were taken and those that were returned.

### This is the first release.
Meta Team Time Data Report Distributed under the GNU General Public License v3.0. See LICENSE for more information. https://github.com/Edwin-Kutsushi/Moringa-DSC-week-2-IP.git

### Contributing

Fork it https://github.com/Edwin-Kutsushi/Moringa-DSC-week-2-IP.git
Create your feature branch (git checkout -b feature/fooBar)
Commit your changes (git commit -am 'Add some fooBar')
Push to the branch (git push origin feature/fooBar)
Create a new Pull Request
