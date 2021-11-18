# Marketing Mix Models (MMM)

Media Mix Modeling (MMM) can be thought of as the big brother to Attribution Modeling. **Traditionally, MMM is a top-down approach used to assess how to best allocate spend between channels on a macro level.**

MMM assesses the cause and effect of changes to the marketing mix, creates **response curves** for each channel and then uses that information to determine the most efficient combination; **determining ROI from each channel**, and **predicting expected returns** from future media spend.

MMM uses probabilistic methods (like regression) while MTA is more deterministic. &#x20;

> What are we mixing? \*Channels\*. This is all about deciding which channels to spend on, and how much.  Although the MMM analysis itself may include other external factors such as consumer sentiment, economic indicators, seasonality, etc.

Marketing efforts of each channel are not homogeneous, with different ad formats, delivery mediums and creative types used across multiple channels.

MMM’s key strength lies with its ability to analyze offline variables that affect media performance: **market elasticity, marginal profit, point of diminishing returns, seasonality** and how other media impacts consumer behavior.

When done properly, MMM takes historic data into account, and is usually performed once a year (although some companies run it on a quarterly basis).

Traditionally, MMM has been the best fit for brands that focus more on offline channels, but those lines are blurring in today’s digital age as companies across the board integrate their offline and online media channels.

## Adstock

MMM models also tie in the concept of **Adstock**, which measures the cumulative (and decaying rate of) effect of advertising on consumer behavior over time.  &#x20;

Using the concept of _half-life, _and standard models to estimate effects such as **exponential decay model** and the **logistic growth model.**

(See the Zenith deck "MMM How-To")



## Resources

{% embed url="https://medium.com/@BenHinson/understanding-the-difference-between-digital-attribution-and-media-mix-modeling-c4f7b7a53bbc" %}

{% embed url="https://www.amazon.com/s?k=market+mix+modeling&bbn=1000&qid=1302897164&rnid=1000&ref=sr_nr_n_0" %}
Some recommended books for building marketing analytics models in R.
{% endembed %}



## Techniques

[Media Mix Modeling in R | Henry Wang](https://henrywang.nl/media-mix-modeling-in-r/)

A simple example using Kaggle data, set up as a multivariate linear regression problem in R.

* Considerations for possible collinearity
* The coefficients of the linear regression equation give the weight of each channel’s contribution to Sales.



[Marketing Mix Modeling Explained – With R | Gabriel Mohanna’s Blog](https://analyticsartist.wordpress.com/2014/08/17/marketing-mix-modeling-explained-with-r/)

A GREAT example with additional complexities, specific instructions and guidance.

* Transform variables to account for the “memory effect “ of advertising (i.e. advertising’s impact from a given period extending over multiple sales periods) aka the ‘adstock’ effect.
  * [Advertising Adstock – Concept & Formula | Gabriel Mohanna’s Blog](https://analyticsartist.wordpress.com/2013/11/02/calculating-adstock-effect/)
  * [Adstock Rate – Deriving with Analytical Methods | Gabriel Mohanna’s Blog](https://analyticsartist.wordpress.com/2014/01/31/adstock-rate-deriving-with-analytical-methods/)\

* diminishing returns of advertising.
  * [Advertising Diminishing Returns & Saturation | Gabriel Mohanna’s Blog](https://analyticsartist.wordpress.com/2015/03/08/advertising-diminishing-returns-saturation/)



[How Media Mix Modeling Leads To Smarter Ad Spend Decisions 2021 Update](https://tinuiti.com/blog/data-privacy/media-mix-modeling/)

Annica’s approach includes additional factors, and speaks to implementing MMM, forecasting and measuring with holdout, etc:

* Segmenting by market, tactic, time of year.
* Folding into forecasts that factor in seasonality (Arima), macroeconomic and competitive data.
* Competitive analysis from providers like Kantar and Pathmatics
* Consumer/Business Confidence, Consumer Sentiment Indexes
* S\&P 500 Trends, Volatility Index
