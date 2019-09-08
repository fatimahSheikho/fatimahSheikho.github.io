---
layout: post
title: New York Subways Traffic Analysis
---



# Introduction:
 
WomenTechWomenYes (WTWY) international company has an annual gala at the beginning of the summer each year, and they asked us to analyze the MTA data, to distribute their teams among the top stations in New York to collect as much signatures as possible. 




# Methodology:

 #  1.	Data acquisition
 
We chose the data of May and August 2019 from [MTA ](http://web.mta.info/developers/turnstile.html). The dataset has 14 columns. 378 stations, 469 Units, and 224 SCP’s.

# 2.	Data Cleansing
 
 To prepare the data before processing it we did some steps:

-We concatenated “Data and Time” column into one, also we dropped some of the columns that we did not need while processing the data, the columns are: C/A, LINENAME, DIVISION, DESC.

-We created a unique identifier called (DUS) for each turnstile (Station, SCP, UNIT), it will help in calculating the average traffic time.

-We added a ‘hour’ column that gets the hour from time, to know the average traffic per hour in weekends and weekdays.

- We striped out all the white space, dealt with missing values, and calculated the exact number of exits and entries. 
![image]({{site.url}}/images/Screen Shot 2019-09-07 at 10.48.44 PM.png)


#  3.	Data processing

Firstly, we calculated the total number of traffic= entries + exits, the number of entries and exits per hour, and the average, sum and max. 
![image]({{site.url}}/images/Screen Shot 2019-09-07 at 11.15.58 PM.png)


We sorted the data based on the unique identifier ‘DUS’ and from the average total of traffic we took top five stations in May and August. With the help of Seaborn we plotted the results.
![image]({{site.url}}/images/Screen Shot 2019-09-07 at 8.31.08 PM.png)
![image]({{site.url}}/images/Screen Shot 2019-09-07 at 8.31.28 PM.png)


Lastly, we calculated the average traffic per hour in weekends and weekdays.

![image]({{site.url}}/images/Screen Shot 2019-09-07 at 8.31.40 PM.png)
![image]({{site.url}}/images/Screen Shot 2019-09-07 at 8.31.47 PM.png)
# 4.	Results

Lastly, we suggested the topmost traffic station in May which is BAYCHESTER AV, and Dekalb AV in August. Also, it is preferable to signatures collect in the afternoon during weekdays, and evenings during the weekends. So far, the project was so challenging, yet, I enjoyed every minute working on it. I have learned how to use Pandas and Seaborn and apply them in my project.




