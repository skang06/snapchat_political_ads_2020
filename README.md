# Factors Affecting Number of Impressions on Snapchat Political Ads in the United States for the 18-40 Age Bracket 
## Background
Recently, Snapchat has been "actively going after" political ads, according to Jeremi Gorman, Snap's chief business officer, in a Quarter 2 Earnings call in July. According to the [article](https://mashable.com/article/snapchat-political-ads-q2-2020-earnings/), Snapchat's predilection for political ads goes against peer social media companies, like Twitter. It is interesting to see how they make be effecting voters in the upcoming election.

A look into data from [Snap Political Ads Library](https://www.snap.com/en-US/political-ads/) will help us understand the reach and scope of Snapchat ads.

## Business Question
___How can effective are political ads on Snapchat?___

## Open Data 
__Snap Political and Advocacy Ads Library:__ this library contains all the political and advocacy ads that Snap runs on their platform. A full data dictionary of column variables can be found [here.](https://github.com/skang06/snapchat_political_ads_2020/blob/master/readme.txt)
- [Snapchat Political Ads 2020](https://github.com/skang06/snapchat_political_ads_2020/blob/master/PoliticalAds.csv):this dataset contains the original data source

## Data Analysis 

1.__How does the number of days the ad was in use affect the number of impressions?__

![alt text](https://github.com/skang06/snapchat_political_ads_2020/blob/master/days_used.png)

The simple linear regression line with the number of days used as the independent variable only accounts for approximately 3% (R squared value of .03) of the data.

![alt text](https://github.com/skang06/baltimore-nassau-county/blob/master/nassaupivot1.png)

We did another analysis with the other independent variable amount spent on the ad. The simple linear regression line shows that 78% of the data is accounted for by the line. 

2. __Can you predict the number of impressions for an advertisement based on whether it starts on the weekend, amount spent on the ad, and days that it was used for based on Snapchat ad data for the United States from 2020?__

- A multiple linear regression found that starting on a weekend was an insignificant variable because it had a p-value of .74 which is greater than .05. This means that there is reason to believe that the null hypothesis is true. Null hypothesis states that there is no relationship between the independent and dependent variables. This is true for starting on the weekend and number of impressions.

3. __Can you predict the number of impressions for an advertisement based on the amount spent on the ad and days that it was used for based on Snapchat ad data for the United States from 2020?__

- A multiple linear regression was taken with amount spent on the ad and the days that the ad was used for (since weekend start was insignificant). There were p-values of >.001 and 1.49 x 10^-7. Both of which are less than .05. This shows that the amount spent and days live are both statistically significant variables that affect the number of impressions.

- _The multiple linear regression equation is number of impressions = -331958 + 294 * amount spent + 8455 * days used._

- The R Square value of .788 means that 78.8% of the number of impressions could be attributed to the multiple lineer regression line with spending and the number of days the ad was live for as the two independent variables. This means that the amount spent on the ad and number of days the ad is live are very crucial for Snap political ads. This shows that this multiple linear regression shows the predicted equation as a good fit for the given equation

- The standard error is at 1,724,551 impressions. This is similar to standard deviation, and measures how spread out the number of impressions for ads on Snap are. The number of d [FINISH]

- This is a good F-significance at 0 because it is low, which indicates that the probability that none of these variables matter in determining the number of impressions of F is basically 0. In other words, the amount spent and the number of days used is significant in helping determing the number of impressions that an ad might get.

- Just how significant can be figured out by the coefficients. The coefficient in front of amount spent signifies that a one dollar increase in amount spent will increase the number of impressions by 294, holding amount of days used constant. The coefficient in front of days used signifies that a one day increase in days the ad was used, increases the number of impressions by 8455, holding amount spent constant. This demonstrates that the number of days the ad was used was very important in increasing the number of impressions. However, the amount of 

Thus, this can help political organizations figure out how much to spend on an ad they might want to buy and how long they should keep it live for. This is particularly important and of use now. Given how close we are to election day, at the moment, it could also help organizations figure out whether it might be worth it to them to buy a short term ad. It could help them weigh the different factors of price and time in determining effectiveness of election ads they choose to roll out in the coming days and weeks. For the future, it could help political organizations roll out ads reallly early. Even cheap ones. As they seem to have a greater effect.


This also helps provide color on whether cost is more important than longevity for an ad on Snapchat. 
what additional data: A deeper look into why the simple linear regression shows a greater significance of price than number of days the ad was used could be a nice place to start.

## Summary
It is important because 


