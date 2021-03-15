# Lyft Bike Trips Dataset Exploration
## by Rongrong Liu


## Dataset

> This dataset contains ride_id and other aspects of a trip for approximately 138,000 bike trips in 05/20 from Lyft.There are 138251 trips in the dataset with 14 features ('ride_id', 'rideable_type', 'started_at', 'ended_at', 'start_station_name', 'start_station_id', 'end_station_name','end_station_id', 'start_lat', 'start_lng', 'end_lat', 'end_lng','member_casual', 'is_equity'). Only four variables are numeric, the rest of them are all categorical including the start_station_id and end_station_id.

## Summary of Findings

> In this exploration I found that: generally, almsot 80% of the bike trips fall in 30 mins, there're noly 20% of the trips beyound 30 mins. When the duration increads, the trips accordingly decreases. The trips using a docked bike are only half of the electric bikes. The Member trips are only 2/3 of the Casual trips. The most trips happen around 5pm to 6pm, and during 2am to 5am, the trips are least. 

> The trips use a electric bike are more than twice than trips use a docked bike, but the duration range of elctric_bike is a little shorter than docked_bike.The trips made by members are much less than the trips made by customers, and also the proportion of the within 30mins trips for the casual is bigger than that for the member. There are more trips last longer than 50mins. The trip duration gets its peak at around 12pm. Overall the trips after 12pm have a bigger duration than the ones before 12pm, and have more longer duration trips. All trips start from two main lantitude: one is around 37.3, another is around 37.8. There are more trips happen around 37.8. Lantitude 37.7-37.9 is the main area where trips stopped.All trips end at two main longitude: one is around -122.4, another is around -121.9. There are more trips end at around -122.4. Lantitude -122.5 to -122.2 is the main area where trips stopped.
From the two plots above, we can see there are two main areas we can use Lyft bike, one is (lat 37.8, lng -122.4), another one is (lat 37.3, lng -121.9).

> The number of member trips is much less than the number of customer trip. For electric_bike, there's no big difference of the distribution of customer and member, just the trip amount of customer is two times than member. For docked_bike, the trip amount is almost the same, but not like member, the customer prefers longer trips. Overall the docked_bike trips last longer than the electic_bike trips. There are a lot of docked_bike trips acually last 1400 mins. There's no big difference for the electric_bike trips durations according the start time, however, it's not the same for docked_bike trips. The durations for customer trips are longer than member trips durations, this is may becuase that we have more customer trips. But the members trips have more superlong trips around 1400 mins, and evenly distributed according the start times.

## Key Insights for Presentation

> In this presentation, I focus on the trip differences of the member trips and the customer trips. First, I use a histgramp to check the overall trip duration distribution. The distribution of the start time. Then to check the trip amount and duration have any differences on different bike types, I use a subplot to seperately plot the trip distribution on electric bikes and docked bikes. Used a scatter plot to plot the relationship of the trip durations and the start times. At the end, I add a row in the subplot, it's member_casual to see if the members have any differences on trip durations and trip amounts. For different bike types, the distribution of the trip durations and the start times. For members and customers, the distribution of the trip durations and the start times.