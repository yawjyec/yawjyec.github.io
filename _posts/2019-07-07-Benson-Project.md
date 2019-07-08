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

The data extracted from MTA website needed some cleaning before we could use it for further analysis. This is in fact an excellent data for us since it made us aware that real world data is normally messy and inconsistent. 

In order to find out the ridership of all subway stations, we used the turnstiles' entries and exits values. Since the values were not commuter counts at that particular hour, but turnstile counter values, we had to extract the counts by subtracting value from one row before.

![Image test]({{ site.url }}/images/MTA_Data_Raw.png)

## Analysis

We started the analysis by studying commuter traffic based on the days of the week and the hour of the day. We noticed that weekends had significantly lower ridership compared to weekdays. Based on that, we removed weekends data for further analysis. We also noticed the inconsistency of hour when data was recorded. Therefore, we created two hour-bins to represent the AM rush hour bin and PM rush hour bin. 

Further analysis revealed that PM rush hour (4pm to 8pm) and mid-week (Tuesday, Wednesday and Friday) had the highest ridership. 

![Image test]({{ site.url }}/images/MTA_AM_PM_Compare.png)
![Image test]({{ site.url }}/images/MTA_DayofWeek_Compare.png)

The top five stations that had the highest traffic were identified:
* 34 ST-PENN STA
* GRD CNTRL-42 ST
* 34 ST-HERALD SQ
* TIIMES SQ-42 ST
* 23 ST

Not only were they high in traffic, but they also had low variability. Therefore if our client places their street team at those stations, they are guaranteed to meet with large number of commuters. 

![Image test]({{ site.url }}/images/MTA_Top5_Station1.png)

![Image test]({{ site.url }}/images/MTA_Top5_Station2.png)

## Conclusion

In conclusion, we recommend customer to place their volunteers at the top five station that we identified, during mid-week between 4PM and 8PM.

For more details of the analysis or source code, you can go to [this link](https://github.com/jporcaro1771/Gala_Project/blob/master/Project%20Benson.ipynb)

