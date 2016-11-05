---
layout: post
title: Can analytics help us identify critically acclaimed movies?
---

I have always been a fan of all the Hollywood classics that is so deeply ingrained in American culture. Casablanca, The Bridge of the River Kwai, Star Wars, Jaws, and many other movies are staples of American cinema. It may be obvious now that these movies are spectacular, but before these movies were produced people had no idea whether their audience would like the movie. Production companies would sign famous actors and directors to attract a bigger audience, but often these two factors doesn't mean the movie will be critically acclaimed. I was curious to see if there was any way we can predict the score of a movie before it is released. Therefore, I decided to look at the web for data and see which factors are the most important in producing a quality movie. 

I started by scraping data from the <http://www.boxofficemojo.com/> and <http://www.imdb.com/>. Luckily, there was already a data set on Kaggle that scraped all the important features of a movie on <http://www.imdb.com/>. After scraping from <http://www.boxofficemojo.com/> and downloading the kaggle data set I realized that the IMDB data set already had all the information that was available on boxofficemojo so I just focused on the IMDB data set.

I first looked at the distribution of the IMDB scores to determine which score thresholds were considered as high quality, average, and low quality films. The top 250 movies have a score higher than 8 which is where most of the classic movies have. Memorable movies have a score between 7 and 8. Mediocre movies have a score below 7. 

![alt text]({{ site.baseurl }}/images/Selection_016.png)

After exploring the data set I saw that there were movies from all over the world. There were movies from India, China, Japan, Brazil, and many other countries. I was only interested in American films so I decided to remove them from my data set. This also took care all the different curriences that was in my data set, but only focusing on the dollar.

![alt text]({{ site.baseurl }}/images/Selection_019.png)

I 

![alt text]({{ site.baseurl }}/images/Selection_021.png)


![alt text]({{ site.baseurl }}/images/Selection_020.png)


