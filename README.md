# Google Data Analytics Capstone: Cyclistic Case Study



## Introduction

In this case study, I will perform many real-world tasks of a junior data analyst at a fictional company, Cyclistic. In order to answer the key business questions, I will follow the steps of the data analysis process: Ask, Prepare, Process, Analyze, Share, and Act.


### Power BI Concepts Applied

- ETL Process: Leveraged Power Query for efficient data extraction, transformation, and loading.
- DAX Concepts: Employed calculated and custom columns to derive meaningful insights.
- Data Modeling: Utilized a single-table approach for streamlined analysis.


## Problem Statement

How do annual members and casual riders use Cyclistic bikes differently?

### Business Task

Develop targeted marketing strategies to convert casual riders into annual members.

### Data Source

I used Cyclistic’s historical trip data to analyze and identify trends from Oct 2022 to Oct 2023 which can be downloaded from [divvy_tripdata](https://divvy-tripdata.s3.amazonaws.com/index.html). 


### Data Exploration

![](Data_explore.png)


### Data Processng

- Combined 12 CSV files using Power Query.
- All the rows having missing values were deleted.
- Extracted Month of year, Day of week and Year from the started_at column. 
- Performed analytical transformation of the dataset by adding a custom column "trip Duration."
- Trips with duration less than a minute and longer than a day are excluded.
- A Total 1,375,912 rows were removed in this step.
- Created a month order and day order column to assist with visualization of the data.

  
## Key Insigts 

Bike Usage Patterns of Casual vs. Membership Riders report from Oct 2022 - Oct 2023 

![](Divvy_bikeshare_report.png)

- Total Trips: Members - 3 million, Casual Riders - 2 million.
- Average Trip Duration: Members - 12 mins, Casual Riders - 16 mins.
- Popular Bike Types: Classic bikes dominate for both, but casual riders also use docked bikes occasionally.
- Daily Trends: Both rider types have longer trips on Saturdays and Sundays.
- Hourly Peaks: Members peak at 8 am and 5 pm; casual riders show a steady increase, peaking at 5 pm.


### Geospatial Analysis

![](Divvy_bikeshare_map.png)

Using the Lat and Long data points provided in the dataset, I was able to generate a map showing us the start station with the most trip durations.
I used start stations because the end station points provided a nearly indentical visual to that of the start station so the insights generated from both were thesame.

The grey circles on the map represent the stations, the larger the raduis of that circle the more the total trips were taken from that particular station.

- Noted that inner-city stations are popular among members, coastal stations are favored by casual riders.
- Zooming in further into the maps, we realized the stations located closer to the universities and around the downtown areas were used by a majority of member riders, while those closer to muesems and parks 
  were used by a majority of the casual riders.

  ![](Zoomed_map.png)

- The visual above shows us a zoomed in image of the station with the most trips, we notice that stations around the Univervity of Chicago school of medicine and the main camous of the University of Chicago had 
  the station with member rider trips, while the stations around Gateway park and the Chicago Lakefront trail was more popular amongst the casual riders.


  ## Recommendation

- Weekend Membership Promotions: Introduce weekend-specific membership plans aligned with common hours on Thurs-Fri and Sat-Sun.
- Enhance Coastal Station Experience: Offer amenities and highlight scenic routes to attract more recreational riders as members.
- Event Sponsorship and Activation: Organize biking activities around museums and parks to engage the community.
- Membership Rewards Program: Introduce reward programs for members who consistently use the service during peak hours on the weekend.
- Strategic Partnerships: Forge partnerships with universities and businesses in downtown areas to promote memberships among students and professionals who aren't already members.
  

  







  
 
