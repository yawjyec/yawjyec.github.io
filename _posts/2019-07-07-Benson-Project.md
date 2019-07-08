---
layout: post
title: First Week @ Metis - Project Benson
---

First week at Metis Data Science bootcamp has just ended. It was exactly what I thought it would be... very intense and a lot of new things to learn in a short period of time. For me, the most challenging new tool that I learned has got to be Git and GitHub. I'm still not too familiar with the workflow. Hopefully with more practice, it will come naturally to me in no time.

Did I not mention that this Metis's curriculum is very intense already? Yup... this week, we already had our first project to complete in 4 days. I worked with 3 awesome team members (Hari, Joel and Leo) to analyze MTA subway traffic data. The goal of this project was to help a non-profit client to optimize the placement of their street teams at subway stations, such that they could get as many potential commuters as possible to attend the gala. We went through the EDA (Exploratory Data Analysis) process in order to gain insight of the turnstile data extracted from MTA website.

![Image test]({{ site.url }}/images/MTASubway_hero.jpg)

## Tools

Some of the tools that we used for this project include:
* Pandas
* Numpy
* Matplotlib
* Seaborn
* Pickle 

## Data Extraction and Cleaning

The data extracted from MTA website needed some cleaning before we could use it for further analysis. This is in fact an excellent data for us since it made us aware that real world data is normally messy and inconsistent. We used the turnstiles' entries and exits counts to find out the ridership of all subway stations. 

![Image test]({{ site.url }}/images/MTA_Data_Raw.PNG)

## Analysis

The approach that my team used was to identify the days of the week and time of the day with high traffic first before we narrow down to top 5 stations. our finding showed that PM rush hour (4pm to 8pm) and weekdays had the highest ridership.

![Image test]({{ site.url }}/images/MTA_AM_PM_Compare.PNG)
![Image test]({{ site.url }}/images/MTA_DayofWeek_Compare.PNG)

The top five stations that had the highest traffic are:
* 34 ST-PENN STA
* GRD CNTRL-42 ST
* 34 ST-HERALD SQ
* TIIMES SQ-42 ST
* 23 ST

Not only were they high in traffic, but they also had low variability. Therefore if our client places their street team at those stations, they are guaranteed to meet with large number of commuters. 

![Image test]({{ site.url }}/images/MTA_Top5_Station1.PNG)

![Image test]({{ site.url }}/images/MTA_Top5_Station2.PNG)

```
---
layout: post
title: Jay's Test Post
---
```

Part in the post to tell the page how to title your post and how to render it.

Below are some examples of loading images, making links, and doing other
markdown-y things.


[This is a link](http://thisismetis.com)

![Image test]({{ site.url }}/images/AlanLeeShireGandalf.JPG)

### Other things
* Like
* lists
* and 
* stuff
