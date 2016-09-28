---
layout: post
title: Optimizing staff allocation to produce the greatest exposure to target demographic
---

  For my first data science project I had to create a viable solution for a hypothetical scenario where an organization called WomenTechWomenYes (WTWY) is seeking advice to find interested individuals to partipate in their annual gala and to build awareness for their cause. They would place street teams at entrances to subway stations. The street teams would collect email addresses and those who sign up are sent free tickets to the gala.

  The MTA transit system of New York is enormous. To send staff to every subway station is impractical so my job was to find data online and to engage in exploratory data analysis to come up with recommendations of where to deploy WTWY's staff. My first hypothesis was to see where the biggest traffic of people occured. However, the people of New York is known to be extremely diverse where you can find virtually every personality that you can think of. So I thought to take the demographics around the train stations into account. Therefore, there were two parts of my analysis. One was to see the total traffic of each station and another was to analyze the demographics around each station. 

  My first step was to explore the MTA Turnstile data set that is provided on http://web.mta.info/developers/turnstile.html. My group decided to analyze all the data that was provided on the website which ranged from September 2016 to May 2010. However, we chose to only focus on the months leading up to the gala which was in June so we decided to only look at April, May, and June. Cleaning the data was extremely difficult because it was extremely messy. I did not expect to encounter this much difficulty in doing so. I now know why most data scientists say that they usually spend 80 percent of their time cleaning the data. I learned tremendously on how to clean data from struggling with this data set. I also have to give thanks to Dave, Megha, and Yao who were all in my group. The picture below shows a bar graph of the stations with the most traffic from March until June. We can see that these are the major train stations of the city where a large amount of people commute to enter the city. 

![alt text]({{ site.baseurl }}/images/traffic_by_month.png)

After finding this out we decided to analyze what time of day were the stations seeing the most traffic. My hypothesis was that these stations were busy during the commuting hours. The following graph confirmed my hypothesis.

![alt text]({{ site.baseurl }}/images/traffic_by_hour.png)

After finding out when and where the most traffic was occuring we then decided to analyze the demographics of NYC by zip code. We decided that the people that are most prone to donating and listening to the organization's cause fall under these categories: females, high income and, work's in the tech industry. We pulled data from the Census and OpenSecrets to see where was the highest concentration of people with these traits. The graph below shows the zip codes of people who are most likely to donate with the clearest color being the highest chance.

![alt text]({{ site.baseurl }}/images/demographic.png)

Finally after looking at both graphs we were able conclude where to deploy WTWY's staff. The 5 stations are 14th Street Union Square, 59th Street lines 456QNR, 72nd Street lines 123, 66th Street Lincoln Square, and 49th Street - 7th Ave. These recommendations were generated after taking traffic and demographics into consideration. 
