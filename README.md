# moneytweet
_See the influence of current social trends on the share market._

For more information visit our website: [moneytweet.github.io](https://moneytweet.github.io/)

<br>
<br>

## Functional overview

Shares are an important measure under financial domain. They represent an economic part of a company. However, share prices are not only dependent on the company itself but rely strongly on traders. If lots of them buy a company's share its value rises. If they sell it, the value drops.

Traders follow the interest to sell their shares for a higher price than they bought them with. As a result, they do not only influence a share's price but also rely on it. The difficult part for a trading person is to know when to sell a share. However, knowing this is not exactly possible as other influences may trigger a sudden change of a share's price. Thus, trading is more of a guess.

As traders are people, they are being influenced by daily happenings. A sudden set of a trend could rise a company's share prices. A big platform that does not only sets trends but also gives an overview of current trends is Twitter. Users are able to post their opinion abous any subject. Often, they communicate about trends.

Combining both areas, it should be possible to analyze whether a social trend and a share's price do correlate. This is being done by analyzing the sentiment of tweets belonging to a certain topic and comparing the average mood to the current price of a share. Tweets do probably not influence a share directly but rather represent people's opinion e.g. towards its company. If both share a certain connection, a positive sentiment of a specific amount of tweets and a rise of a share's price should happen in the same time range.

<br>
<br>

## Technical overview

Analyzing a correlation of a social trend and prices of shares needs large amounts of data. Firstly, specific data has to be collected. Share prices can be queried using finance endpoints. Tweets can be collected from APIs provided by Twitter itself. However, this topic cannot only be approached by taking current data. Furthermore, historical data has to be used. In this way, past trends can be identified and used for learning how they represented the trend's influence on a share. Using this data, a model can be developed to adapt historical occurences and using them to identify current and possibly future developments.

By using large amounts of data, a specific data architecture has to be used. Therefore, a Lambda-inspired architecture design has been developed. It focuses on fast data processing for real time data analytics as well as computing older data. Identifying a social trend is consequently possible through analyzing the sentiment of tweets of a specific topic. This makes it not only possible to track real-time changes but also use historical data in combination with new one.

Share prices are being collected as well and used to identify sudden changes in their prices. This leads to points in the past when a social trend could have been occurend and impacted share prices. The collected set of important historical points in time can be verified or counterfeit through sentiments of tweets.