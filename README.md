# Factors Affecting Number of Impressions on Snapchat Political Ads in the United States for the 18-40 Age Bracket 
## Background
Recently, Snapchat has been "actively going after" political ads, according to Jeremi Gorman, Snap's chief business officer, in an Earnings call in July 2020. According to the [article](https://mashable.com/article/snapchat-political-ads-q2-2020-earnings/), Snapchat's predilection for political ads goes against peer social media companies, like Twitter. It is interesting to see how they make be affecting voters in the upcoming election.

A look into data from [Snap Political Ads Library](https://www.snap.com/en-US/political-ads/) will help us understand the reach and scope of Snapchat ads.

## Business Question
___How can effective are political ads on Snapchat for the 18-40 age bracket in the United States?___

## Open Data 
__Snap Political and Advocacy Ads Library:__ this library contains all the political and advocacy ads that Snap runs on their platform. A full data dictionary of column variables can be found [here.](https://github.com/skang06/snapchat_political_ads_2020/blob/master/readme.txt)
- [Snapchat Political Ads 2020](https://github.com/skang06/snapchat_political_ads_2020/blob/master/PoliticalAds.csv): Dataset containing original data source

## Data Analysis 

1.__How does the number of days the ad was live affect the number of impressions?__

![alt text](https://github.com/skang06/snapchat_political_ads_2020/blob/master/days_used.png)

The simple linear regression line with the number of days used as the independent variable only accounts for approximately 3% (R squared value of .03) of the data.

![alt text](https://github.com/skang06/baltimore-nassau-county/blob/master/nassaupivot1.png)

We did another analysis with the other independent variable amount spent on the ad. The simple linear regression line shows that 78% of the data is accounted for by the line. 

2. __Can you predict the number of impressions for an advertisement based on whether it starts on the weekend, amount spent on the ad, and days that it was used for based on Snapchat ad data for the United States from 2020?__

- A multiple linear regression found that starting on a weekend was an insignificant variable because it had a p-value of .74 which is greater than .05. This means that there is reason to believe that the null hypothesis is true. Null hypothesis states that there is no relationship between the independent and dependent variables. This is true for starting on the weekend and number of impressions.

- A multiple linear regression was taken with amount spent on the ad and the days that the ad was used for (since weekend start was insignificant). There were p-values of >.001 and 1.49 x 10^-7. Both of which are less than .05. This shows that the amount spent and days live are both statistically significant variables that affect the number of impressions. Additionally, a low F-significance level at 0 indicates that the probability that the amount spent and the number of days used do not matter in determining the number of impressions of F is basically 0. In other words, they are significant in helping determing the number of impressions that an ad might get. 

- _The multiple linear regression equation is number of impressions = -331958 + 294 * amount spent + 8455 * days used._


- With a standard error of 1,724,551 impressions, it seems rather large. However, the average number of impressions on an ad was 836,175 impressions.

- The R Square value of .788 means that 78.8% of the number of impressions could be attributed to the multiple linear regression line with spending and the number of days the ad was live for as the two independent variables. This means that the multiple regression line formed using the amount spent on the ad and number of days the ad is live explain much of the impressions on Snap political ads. 

- Just how significant these variables are can be figured out by the coefficients. The coefficient in front of amount spent signifies that a one dollar increase in amount spent will increase the number of impressions by 294, holding amount of days used constant. The coefficient in front of days used signifies that a one day increase in days the ad was used, increases the number of impressions by 8455, holding amount spent constant. This demonstrates that the number of days the ad was used was very important in increasing the number of impressions, relative to price.

## Summary
Thus, this can help political organizations figure out how much to spend on an ad they might want to buy and how long they should keep it live for. 
Our data indicates that while both number of days and amount spent on the ad are important factors of determining effectiveness, the number of days the ad was used may be more significant. This is particularly important and of use now. Given how close we are to election day, at the moment, it could also help organizations figure out whether it might be worth it to them to buy a short term ad. It could help them weigh the different factors of price and time in determining effectiveness of election ads they choose to roll out in the coming days and weeks. For the future, there is a definite benefit to political organizations in rolling out these ads really early. 

A deeper look into why the simple linear regression shows a greater significance for amount spent than number of days would be intersting. Moreover, a further look into other variables that could lower the standard error would help political organization increase engagement with their election ads.
