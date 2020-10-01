# Factors Affecting Number of Impressions on Snapchat Political Ads From 2020
## Background
Recently, Snapchat has been "actively going after" political ads, according to Jeremi Gorman, Snap's chief business officer, in a Quarter 2 Earnings call in July. According to the [article](https://mashable.com/article/snapchat-political-ads-q2-2020-earnings/), Snapchat's predilection for political ads goes against peer social media companies, like Twitter. It is interesting to see how they make be effecting voters in the upcoming election.

A look into data from [Snap Political Ads Library](https://www.snap.com/en-US/political-ads/) will help us understand the reach and scope of Snapchat ads.

## Business Question
___Can you predict the number of impressions for an advertisement based on information from 2020?___

## Open Data 
1.	__Snap Political and Advocacy Ads Library:__ this library contains all the political and advocacy ads that Snap runs on their platform. A full data dictionary of column variables can be found [here.](https://github.com/skang06/snapchat_political_ads_2020/blob/master/readme.txt)
- [Snapchat Political Ads 2020](https://github.com/skang06/snapchat_political_ads_2020/blob/master/PoliticalAds.csv):this dataset contains the original data source

## Data Analysis 
Define the data-related questions and metrics (using linear regression)
Perform calculations and model-building to answer the data-related questions
simple and a multiple linear regression equation


Can you predict the number of impressions for an advertisement based on whether it starts on the weekend, amount spent on the ad, and days that it was used for?

A multiple linear regression found that starting on a weekend was an insignificant variable because it had a p-value of .74 which is greater than .05. This means that there is reason to believe that the null hypothesis is true. Null hypothesis states that there is no relationship between the independent and dependent variables. This is true for starting on the weekend and number of impressions.

Can you predict the number of impressions for an advertisement based on the amount spent on the ad and days that it was used for?

A multiple linear regression was taken with amount spent on the ad and the days that the ad was used for (since weekend start was insignificant). There were pvalues of 0 and 1.49 x 10^-7. Both of which are less than .05. This shows that the amount spent and days live are both statistically significant variables that affect the number of impressions.

The multiple linear regression equation is number of impressions = -331958 + 294 * amount spent + 8455 * days used.

The coefficients in front of amount spent signifies that one dollar increase in amount spent will increase the number of impressions by 294, holding amount of days used constant. The coefficient in front of days used signifies that a one day increased in days the ad was used, increases the number of impressions by 8455, holding amount spent constant.

The R Square value of .788 means that 78.8% of the number of impressions could be attributed to spending and the number of days the ad was live for. This means that the amount spent on the ad and number of days the ad is live are very crucial for Snap political ads.

The standard error is at 1,724,551 impressions.

F-significance is 0 which indicates that 


Determine what linear regression statistics such as the R2 value, standard error, coefficients, p-value, and F significance mean for your specific data set, and interpret these results for a non-technical audience
Evaluate and interpret your linear regression models and explain to your audience (based on the dataset used and business questions posed) what these values mean and how your audience should consider these values for current and future operations
 

![alt text](https://github.com/skang06/baltimore-nassau-county/blob/master/nassaupoverty.png)

No one who grew up in Nassau County, regardless of the income of the parents, were living in poverty in adulthood. According to my data, Baltimore only had very small levels of poverty for those who grew up with parents with incomes higher than the 25th percentile. However, for those with parents' income in the 25th percentile or less, around 60% ended up in poverty when they were adults. This demonstrates that getting parents in the 50th percentile made a big difference for those in Baltimore. Looking at how to get more people at that level could help result in lower percentages of adults in poverty. 

![alt text](https://github.com/skang06/baltimore-nassau-county/blob/master/nassaupivot1.png)

Both pivot charts show that there are pockets in both locations where household income is lower across all parent income distributions. This provides a direction of where to potentially concentrate resources in a Baltimore-centric soluutino for maximum benefit in the future. 

## Summary
Relate the data findings back to your initial business question and outline what your linear regression model tells us about election ads, city government salaries, etc.
Explaining a phenomenon that we want to better understand
Predicting things about the future related to our data
Deciding what to do about a current strategy decision


