# citibike-challenge


# Dashboard 1

Station Popularity based on Trip Start Counts and Member Type in the Peak Winter (January 2023) and Summer (July 2023) month.

## Dashboard Interactivity

Dashboard is interactive so that user can visualize data for selected parameters like month Jan(1), July(7) and membership type. Dashboard visualization will change based on the selected options.

## Dataset

The data conatins a summary of the 2023 citibike trip data for the months of January and July 2023. The data has been summarized using Pandas pivot table. Summarization helped in reducing file size and also preprocessing data in required dimesions and measures to reduce processing requirements in Tableau Public. It improved the productivity as summarization reduced the time to create visualizations and dashboards using aggregated data.

## Key Focus-Expectations and Trend Observation

***To understand if weather has an overall effect on the popularity of the Trip/Ride start stations. 
### Expectation 

The Trip/Ride counts will significantly decrease in the peak winter (January 2023) month as comapred to the summer (July 2023) month given the inclement weather occurences leading to only very minimal ridership.

### Trend Observation

In the Top 10 stations determined on the basis of ride counts, the Ride/Trip counts are definitely on the lower side in the month of January as compared to the month of July but the counts are not minimal so these are still significant given January trip counts are more than 50% of the trip counts of July.(Ref. Worksheet:T10Stn_Trip_Count)

However, the Bottom 10 stations completely lose their minimal trip/ride counts in January.(Ref. Worksheet:B10Stn_Trip_Count)


***To understand if weather has any effect on the popularity of the Trip start station amomg the two categories of users (members and casual). 
### Expectation 

The proportion of rides in will remain same for both the members and casual users of citibikes.

### Trend Observation

In the Top 10 sations determined on the basis of ride counts, the Ride/trip counts  don't decrease drastically in January for members as compared to the casual riders whose trip counts decreases to low numbers (less than 1000) in case of all but one station (7th Ave & Central park South).(Ref. Worksheet:T10Stn_Trip_Count)

However, all the Bottom 10 stations completely lose their minimal trip/ride counts in January and only 3 out of Bottom 10 stations maintain the minimal trip/ride count of 1 in July.(Ref. Worksheet:B10Stn_Trip_Count)

## Unexpected Finding and Possible Explanation

Zipcode 10001 has 2 Stations that fall in the category of Top 10 with trip counts 17167 and 15611 (Ref. Worksheet:T10_Str Stn (Zipcode)) but it also has 2 stations that fall in the category of Bottom 10 with trip counts as low as 1 and 4 (Ref. Worksheet:B10_Str Stn (Zipcode)). It seems like an anamoly that an area with such disparity in popularity of citibike stations exists within the same zip code. perhaps these stations need to be advertised more or maintained better if that is the reason for their lack of popularity.

Overall, it is also unexpected that there are many stations with minimal trip start counts in Manhattan area as shown on the Bottom 10 map considering Manhattan is a high traffic area.



# Dashboard 2

Popular Ride Hours and Ride Durations among CitiBike Riders in Peak Winter (January 2023) and Summer (July 2023) month.

## Dashboard Interactivity

Dashboard is interactive so that user can visualize data for selected parameters like month Jan(1), July(7) and membership type. Dashboard visualization will change based on the selected options.

## Dataset

The data conatins a summary of the 2023 citibike trip data for the months of January and July 2023. The data has been summarized using Pandas pivot table. Summarization helped in reducing file size and also preprocessing data in required dimesions and measures to reduce processing requirements in Tableau Public. It improved the productivity as summarization reduced the time to create visualizations and dashboards using aggregated data.. 

## Key Focus-Expectations and Trend Observation

***To understand if weather has an overall effect on the popularity of the Ride times in a day based on the sum of ride counts. 
### Expectation 

The peak ride hours will be similar in both early morning, 7 am or 8am and early evening, 5 pm or 6 pm considering the office rush hours. Also the peak hours in January and July will be different, likely earlier in the evening to take advantage of the daylight in January as compared to the peak summer month of July. The member riders are expected to be greater than the casual riders, especially in the peak hours.

### Trend Observation

Peak hours based on the sum of ride counts are 5 pm and 6 pm. None of the morning office hours showed similar ridership as these evening peak hours. Also, unlike the expectation, these peak hours remain same for both the month of January and July. However, as per expectation, member riders are more than the casual riders during peak hours. (Ref. Worksheet:PeakHrsTrpCnts)

***To understand if weather has an effect on the most common trip duration amomg the two categories of users (members and casual). 
### Expectation 

The riders both members and casual, will likely engage in longer duration trips in the month of July as compared to January.

### Trend Observation

The most common Trip duration is between 5-10 mins. Unlike the expectation, in both January and July, this short trip duration remains the most popular among riders. (Ref. Worksheet:MostCmn_TrpDuration)

## Unexpected Finding and Possible Explanation

As the Trip duration increases, the casual members proportion in the total count is increasing(Ref. Worksheet:MostCmn_TrpDuration). This shows that members are using the citibikes for shorter durations while casual riders use the citibikes for longer duration.This usage is likely for excursions and exploring the city by tourists who take advantage of this service. The add to the numbers of the local casual riders. 


# City Official Map - All Bike Stations with Zipcode

## Trends Discovered

### General Activity Levels
January (Month 1): The overall size of the circle markers (representing sum of trip start counts) is much smaller, indicating lower activity levels in January.
This trend aligns with seasonal patterns, as colder weather in January typically reduces outdoor activities like cycling.  
July (Month 7): The circle markers are significantly larger across almost all stations, reflecting higher usage.
Summer months (like July) typically see an increase in outdoor activities, and CitiBike usage tends to peak during these months.

### Geographic Patterns
Both maps show similar geographic coverage, i.e. the network of stations remained consistent in both months.
However, in January, most stations show low usage, with only a few slightly larger markers in busy areas (e.g., Midtown Manhattan or Downtown Brooklyn).
In July, stations across Manhattan and other boroughs show widespread increased activity, with higher usage distributed throughout the city.

### Popular Stations
January: A few stations in central Manhattan (e.g., areas with high commuter or tourist activity) stand out slightly due to consistent year-round demand. Usage is concentrated in key transportation hubs or densely populated areas.  
July: Almost all stations in Manhattan, Brooklyn, and parts of Queens show substantial increases in activity.
Tourist-heavy areas, such as Lower Manhattan and Midtown, experience the highest surge in bike usage.

### Impact of Weather and Seasonality
January: Cold temperatures and possibly snow reduce cycling as a transportation choice, which is why most stations see minimal activity.  
July: Warm weather and longer daylight hours encourage more people to use CitiBike for commuting, recreation, and leisure activities.

### Zip Code-Level Trends
The maps show zip code boundaries with varying levels of bike usage.  
January: Few zip codes, such as 10001 (Midtown Manhattan), show slightly higher activity due to consistent commuter or resident usage.
July: High activity across multiple zip codes, particularly in areas like 10014 (West Village) and 11201 (Downtown Brooklyn), which have well-connected bike lanes and attract significant tourist and local traffic.
