
# Predicting TV Series Ratings

# Purpose:
Being able to predict the rating of TV series before its release. So, it will attract audiences and increase the chance of its  success. From a business perspective, it will attract advertisers to promote their products during the stream of the series.

# Features:

I chose the following features because I thought that they represent TV series well. Features are duration, votes, genres and released year.

# Model Process:

- Web scrapping 

By using beautiful soup tool, I web scraped IMDB website and acquired 1000 TV series.
2- Data cleaning
In this step I dropped all NaN  rows and removed TV Series with  zero  Votes using Pandas as a tool.
 
- Model Training and Validation

Firstly, I split off the data for testing. Then, Create a baseline Model and the score was R^2 = .099, the score is low, for this reason, I started doing feature engineering and build other models and compare them with my baseline. Lastly, I Validated the most suitable models.

- Feature engineering 

I power transformed my target and figures below show residual plot before and after.

![image]({{site.url}}/images/Before_power.png)

![image]({{site.url}}/images/download-1.png)

- Testing 
Tested best performing models, and I chose linear regression as my model with  R^2 = 0.29. 


Notable Coefficients

![image]({{site.url}}/images/coef.png)
# Results:
I concluded that a documentary TV series have a high probability of being highly rated. Also, that duration has a negative correlation with ratings, meaning the less the duration the more the rate.

