# Analyzing New York Citi Bike

<img src="https://i.ibb.co/Lx4WYZ8/citibike-logo.jpg" width="300" height="120">

## About

Created by: Luis E. Rojas

   - This is the project I developed for unit 20 of the Boot Camp: [Data Visualization and Analytics](https://bootcamp.uncc.edu/data/)
   - I created a Tableau Workbook in order to analyze NYC's Citi Bike program during pandemics, as well as help readers understand my findings. For more details, see [here](#the-original-text-of-the-homework-assignment).
   - Here is a snapshot of the workbook: 


<img src="https://i.ibb.co/NNqZyCM/snapshot.png" width="600" height="400">



- ### The workbook's link for this project is [here](https://public.tableau.com/views/CitiBikeAnalytics_16208735130000/CitiBikeStory?:language=en&:display_count=y&publish=yes&:origin=viz_share_link).
- The main tool I used on this project is [Tableau Public](https://public.tableau.com/).


## Overview

<img src="https://i.ibb.co/FWn6TW6/Bikes.jpg" width="600" height="400">

Every month, Citi Bike releases a treasure trove of data that includes information on each individual trip (e.g. duration, start and end location, subscription type, gender of rider). The data is available here - http://www.citibikenyc.com/system-data. I pulled data to study the behavior during 12 months of the covid-19 pandemics (apr’20 to mar’21). I merged the twelve files since they had similar layout. It was a massive dataset that contained over 19 million records. 

<img src="https://i.ibb.co/1R0JjVw/union.png" width="600" height="400">

However, there is a limit of 15 million records handled by the Tableu Public server, that is why I limited and cleaned up the data at the same time. Dropping rows with unknown gender, birth year before 1940 and trip duration below 140 seconds.

<img src="https://i.ibb.co/G5wRfMw/cleanup.png" width="600" height="400">

## Who rides Citi Bikes?

In order to answer this very first question I built a total of 27 worksheets, 7 dashboards and 1 story. Below is the story, which contains a summary of the most important phenomenas.

<img src="https://i.ibb.co/0qQ8TMN/story1.png" width="600" height="400">

Here, as we can notice:
- There are more subscribers than regular customers.
- Since the beginning of the pandemics the ridership has decreased 69%
- There was a high peak between August and October 2020, perhaps caused by the closure of most businesses.

<img src="https://i.ibb.co/gZ0KJVJ/story2.png" width="600" height="400">

According to this:
- Looks like most riders are under 25 years old. There are still many people of all ages, though.
- The older is the rider the fewer minutes spent on the trip.

<img src="https://i.ibb.co/VH71BLC/story3.png" width="600" height="400">

- Seems like men are more interested in biking than women.
- Women have aproximately the same trend to ride on the same age as men.

<img src="https://i.ibb.co/w4hZ8j4/story4.png" width="600" height="400">

- When moving through different months on the NYC Official Map, the number of trips varies. This may be caused by the reopening of businesses.
- The habits to ride at the same time remain almost the same throughout the year.

<img src="https://i.ibb.co/Hxzdw9r/story5.png" width="600" height="400">

- According to this dataset, there are many bicycles that may be due for maintenance. This implies the program has been successful but it needs maintenance.

<img src="https://i.ibb.co/M9dRYP2/story6.png" width="600" height="400">

- Average trip duration is aroung 20 minutes. However, there are some bike stations with and average above 24 hours. It seems that some stations allow subscribers to return the bikes the next day, or maybe their access is restricted on Sundays or Holidays.

<img src="https://i.ibb.co/VHwmCTB/story7.png" width="600" height="400">

- There is a huge gap among some stations with almost no trips and some other with more than 90 thousand trips.
- They seem mixed up in the map, though.

## Conclusion, Summary, and Future Work

According to the data obtained from the website, the Citi Bike program has been successful in New York, and as such, it needs to be overseen closely for any change in the environment.

Because of limitations with time and computing power, even though I did much research on the CitiBike website, I could not contribute all my ideas into the models. From the comprehensive literature review, in the future I could expand the analysis further, such as prediction of aggregate trip fees to determine revenue generation, etc.



## **_The original text of the homework assignment:_** 
# Tableau Homework - Citi Bike Analytics

### Before You Begin

* This assignment will be saved to your Tableau Public account rather than GitHub. 

* If you haven't already, be sure to create a Tableau Public account [here](https://public.tableau.com/s/).

* The free tier of Tableau only lets you save to their public server. This means that each time you save your file it will be uploaded to your Tableau Public profile. 

* You are able to load and continue working on the same workbook.

* When you are finished with your assignment, you will turn in the URL to your Tableau Public workbook along with any additional files used for your analysis. 

## Background

![Citi-Bikes](https://i.ibb.co/VCKfVgn/citi-bike-station-bikes.jpg)

Congratulations on your new job! As the new lead analyst for the [New York Citi Bike](https://en.wikipedia.org/wiki/Citi_Bike) Program, you are now responsible for overseeing the largest bike sharing program in the United States. In your new role, you will be expected to generate regular reports for city officials looking to publicize and improve the city program.

Since 2013, the Citi Bike Program has implemented a robust infrastructure for collecting data on the program's utilization. Through the team's efforts, each month bike data is collected, organized, and made public on the [Citi Bike Data](https://www.citibikenyc.com/system-data) webpage.

However, while the data has been regularly updated, the team has yet to implement a dashboard or sophisticated reporting process. City officials have a number of questions on the program, so your first task on the job is to build a set of data reports to provide the answers.

## Task

**Your task in this assignment is to aggregate the data found in the Citi Bike Trip History Logs and find two unexpected phenomena.** 

**Design 2-5 visualizations for each discovered phenomena (4-10 total). You may work with a timespan of your choosing. Optionally, you may merge multiple datasets from different periods.** 

**The following are some questions you may wish to tackle. Do not limit yourself to these questions; they are suggestions for a starting point. Be creative!**

* How many trips have been recorded total during the chosen period?

* By what percentage has total ridership grown?

* How has the proportion of short-term customers and annual subscribers changed?

* What are the peak hours in which bikes are used during summer months?

* What are the peak hours in which bikes are used during winter months?

* Today, what are the top 10 stations in the city for starting a journey? (Based on data, why do you hypothesize these are the top locations?)

* Today, what are the top 10 stations in the city for ending a journey? (Based on data, why?)

* Today, what are the bottom 10 stations in the city for starting a journey? (Based on data, why?)

* Today, what are the bottom 10 stations in the city for ending a journey (Based on data, why?)

* Today, what is the gender breakdown of active participants (Male v. Female)?

* How effective has gender outreach been in increasing female ridership over the timespan?

* How does the average trip duration change by age?

* What is the average distance in miles that a bike is ridden?

* Which bikes (by ID) are most likely due for repair or inspection in the timespan?

* How variable is the utilization by bike ID?

**Next, as a chronic over-achiever:**

* Use your visualizations (does not have to be all of them) to design a dashboard for each phenomena.
* The dashboards should be accompanied with an analysis explaining why the phenomena may be occuring. 

**City officials would also like to see one of the following visualizations:**

* **Basic:** A static map that plots all bike stations with a visual indication of the most popular locations to start and end a journey with zip code data overlaid on top.

* **Advanced:** A dynamic map that shows how each station's popularity changes over time (by month and year). Again, with zip code data overlaid on the map.

* The map you choose should also be accompanied by a write-up unveiling any trends that were noticed during your analysis.

**Finally, create your final presentation**

* Create a Tableau story that brings together the visualizations, requested maps, and dashboards.
* This is what will be presented to the officials, so be sure to make it professional, logical, and visually appealing. 

## Considerations

Remember, the people reading your analysis will **NOT** be data analysts. Your audience will be city officials, public administrators, and heads of New York City departments. Your data and analysis needs to be presented in a way that is focused, concise, easy-to-understand, and visually compelling. Your visualizations should be colorful enough to be included in press releases, and your analysis should be thoughtful enough for dictating programmatic changes. 

## Submission 

Your final submission should include:

* A link to your Tableau Public workbook that includes: 
  * 4-10 Total "Phenomenon" Visualizations 
  * 2 Dashboards
  * 1 City Official Map
  * 1 Story 
* A text or markdown file with your analysis on the phenomenons you uncovered from the data.

## Sharing Your Work

* In order to share your work, we are asking that you will save your workbook as a .twbx file.

* To save your workbook as a .twbx file, you will just need to go to `File`, then `Save to Tableau Public...`.

* Please create an account if you do not have one already.

* Once you have created an account and published your work to Tableau Public, go to the visualization in Tableau Public and find the `Download` button at the bottom right hand corner.

* Please download the Tableau Public file to your computer and submit it.

## Assessment

Your final product will be assessed on the following metrics:

* Analytic Rigor

* Readability

* Visual Attraction


## Hints

* You may need to get creative in how you combine each of the CSV files. Don't just assume Tableau is the right tool for the job. At this point, you have a wealth of technical skills and research abilities. Dig for an approach that works and just go with it.

* Don't just assume the CSV format hasn't changed since 2013. Subtle changes to the formats in any of your columns can blockade your analysis. Ensure your data is consistent and clean throughout your analysis. (Hint: Start and End Time change at some point in the history logs).

* Consider building your visualizations with small extracts of the data (i.e. single files) before attempting to import the whole thing. What you will find is that importing all 20+ million records of data will create performance issues quickly. Welcome to "Big Data."

* While utilizing all of the data may seem like a nice power play, consider the time-course in making your analysis. Is data from 2013 the most relevant for making bike replacement decisions today? Probably not. Don't let overwhelming data fool you. Ground your analysis in common sense.

* Remember, data alone doesn't "answer" anything. You will need to accompany your data visualizations with clear and directed answers and analysis.

* As is often the case, your clients are asking for a LOT of answers. Be considerate about their need-to-know and the importance of not "cramming in everything". Of course, answer each question, but do so in a way that is organized and presentable.

* Since this is a project for the city, spend the appropriate time thinking through decisions on color schemes, fonts, and visual story-telling. The Citi Bike program has a clear visual footprint. As a suggestion, look for ways to have your data visualizations match their aesthetic tones.

* Pay attention to labels. What exactly is "time duration"? What's the value of "age of birth"? You will almost certainly need calculated fields to get what you need.

* Keep a close eye for obvious outliers or false data. Not everyone who signs up for the program is answering honestly.

* In answering the question of "why" a phenomenon is occurring, consider adding other pieces of information on socioeconomic or other geographic data. Tableau has a map "layer" feature that you may find handy.

* Don't be afraid to manipulate your data and play with settings in Tableau. Tableau is meant to be explored. We haven't covered all that you need -- so you will need to keep an eye out for new tricks.

* Treat this as a serious endeavor! This is an opportunity to show future employers that you have what it takes to be a top-notch analyst. 

* Good luck!

## Rubric

[Unit 20 Rubric - Tableau Homework - Citi Bike Analytics](https://docs.google.com/document/d/135gKIRxE8XB9XGmXcGORGpmJAeGdh1qz6ogh8na6P-o/edit?usp=sharing)

- - -

© 2021 Trilogy Education Services, LLC, a 2U, Inc. brand. Confidential and Proprietary. All Rights Reserved.
