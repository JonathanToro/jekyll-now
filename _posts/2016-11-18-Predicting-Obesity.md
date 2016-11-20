---
layout: post
title: Is your neighborhood fat?
---
Obesity is a serious problem that jeopardizes any individual's well being. Being obese means having a body mass index greater (BMI) greater than 30. This increases the risk of developing a plethora of debilitating health conditions such as coronary heart disease, diabetes, depression, strokes, and even cancer. We often hear in the news about the obesity epidemic in America and how the American culture tends to serve portions of food that is several times more than in other countries. According the the CDC as many as 35 percent of Americans are considered obese. This monumental figure sparked my interest in investigating why is obesity so prevalent in our population. Thus, I looked online for data to see what trends I can find about the population. I found 6 data sets from the Community Status and Health Indicators (CHSI) database that described the demographics, social behaviors, causes of deaths, preventive services use, environmental statistics, and importance of health by county. The data has 3142 counties in total. After looking through the data I saw that the obesity rate for around 30% of the counties was missing. I found this alarming. Therfore, I decided to predict whether these missing counties were above or below the median obesity rate.

The graph below was made using d3.js and visualizes the counties' obesity rates. The darker the blue means that there is a higher obesity rate. The gray means that data is missing for these areas.

![alt text]({{ site.baseurl }}/images/Selection_027.png) 

The chart below shows the distribution of obesity rates in the counties. The median is around 24% and the mean is around the same.

![alt text]({{ site.baseurl }}/images/Selection_028.png)

Another visualization of the obesity rates by state. 

![alt text]({{ site.baseurl }}/images/Selection_029.png)

Combining all the data sets gave me around 500 features. There are only 3142 counties so I had to reduce the dimensionality of the data. I did so by adding random noise to the data and running a random forest several times to determine the most important features that contribute to obesity rates. 
![alt text]({{ site.baseurl }}/images/Selection_030.png)

![alt text]({{ site.baseurl }}/images/Selection_031.png)

![alt text]({{ site.baseurl }}/images/Selection_033.png)
