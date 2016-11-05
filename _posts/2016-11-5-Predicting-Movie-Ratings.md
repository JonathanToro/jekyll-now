---
layout: post
title: Can analytics help us identify critically acclaimed movies?
---

I have always been a fan of all the Hollywood classics that is so deeply ingrained in American culture. Casablanca, The Bridge of the River Kwai, Star Wars, Jaws, and many other movies are staples of American cinema. It may be obvious now that these movies are spectacular, but before these movies were produced people had no idea whether their audience would like the movie. Production companies would sign famous actors and directors to attract a bigger audience, but often these two factors doesn't mean the movie will be critically acclaimed. I was curious to see if there was any way we can predict the score of a movie before it is released. Therefore, I decided to look at the web for data and see which factors are the most important in producing a quality movie. 

I started by scraping data from the <http://www.boxofficemojo.com/> and <http://www.imdb.com/>. Luckily, there was already a data set on Kaggle that scraped all the important features of a movie on <http://www.imdb.com/>. After scraping from <http://www.boxofficemojo.com/> and downloading the kaggle data set I realized that the IMDB data set already had all the information that was available on boxofficemojo so I just focused on the IMDB data set.

I first looked at the distribution of the IMDB scores to determine which score thresholds were considered as high quality, average, and low quality films. The top 250 movies have a score higher than 8 which is where most of the classic movies have. Memorable movies have a score between 7 and 8. Mediocre movies have a score below 7.

The data had around 30 features which included budget, gross, actors, actresses, country of origin, year of release, and many more. I tested out these features with a linear regression model and only achieved a R-squared value of 27.7%. I tested the data with other models such as ridge models, adaptive boosting, lasso models, random forests, and gradient boosted regression. My best model turned out to be from using gradient boosted regression that achieved a R-squared value of 42.6% which is still isn't great, but at least it's an improvement from the linear regression model. I introduced random noise into the model so I can throw out the features that aren't important. I also tried some feature engineering such as introducting a dummy variable if the director was casted in more than 95% than other directors then from 60% to 95% then from 60 and below. However this feature engineering didn't work. In the end I found out that the most important features to determining the IMDB score were movie facebook likes, director facebook likes, duration, and the budget of the film. 

![alt text]({{ site.baseurl }}/images/Selection_016.png) 



![alt text]({{ site.baseurl }}/images/Selection_022.png)


![alt text]({{ site.baseurl }}/images/Selection_025.png)


![alt text]({{ site.baseurl }}/images/Selection_024.png)




