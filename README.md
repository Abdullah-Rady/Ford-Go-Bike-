# (Ford GoBike System Data Exploration)



## Dataset

> GoBike Data is a dataset for bike trips happened on 2019, Each trip is includes:-
- Trip Duration (seconds).
- Start Time and Date.
- End Time and Date
- Start Station ID.
- Start Station Name.
- Start Station Latitude.
- Start Station Longitude.
- End Station ID.
- End Station Name.
- End Station Latitude.
- End Station Longitude.
- Bike ID.
- User Type (Subscriber or Customer – “Subscriber” = Member or “Customer” = Casual).

> befor we start our exploration we made some data wrangling:-
- convert start_time, end_time from object to pandas Datetime.
- convert user_type, start_station_name, end_station_name from object to category.
- extract month, dayofweek and hour from the start_time and save them in separate columns.
- remove null and duplicated values.

## Summary of Findings

> during the exploration of the dataset I found that:-
- the most common duration time is from 0 to 500 secounds.
- We can see that Market St at 10th St is the most common start station.
- The number of subscribers is more than Customers.
- We can see that the majority of users are males.
- By looking at these plots we can say that most frequent users of bikes are aged between 20 and 45. Higher duration is clocked by      younger members.
- We can see that all of the rides were made in February.
- We can see that although the number of customers is fewer than subscribers their average time is heigher.
- Subscribers predominately use the ride service on Monday through Friday, while customers ride the most on the weekends.
- during all days of week the median (duration) of customer type is higher than the median (duration) of subscriber type.
- Saturday has the most bikers in customer type.
- There is a jump in duration for others at an older age (around 60 years).
- In all gender types, the age range of 10-20 has the longest trip duration, this is maybe due to the young age still has more stamina, so they tend to ride the bikes longer either for recreation or for school.


# Key Insights for Presentation

- For the presentation, I collected all of the plots and results that I found and made a slide for each one.
- I start by introducing the all of the univariate plots then bivarite and mutivariate plots.
- Afterwards, I introduce each of the categorical variables one by one. To start, I use histograms to plot the distribution of some variabes like age and duration. for bivariate plots I use boxplots and scatter plots.

- Gender has no real effect on ride duration. One might expect that males would be taking the longest  rides, but the data doesn't indicate this at all. Across all ages, the differences between duration of male riders vs. female & other riders is negligible. In fact, it wasn't uncommon that females and those who marked their gender as "Other" would often ride longer than male riders.

- Folks in their early 30's comprise the bulk of the rides. This one is the one that surprised me the most. Knowing that people as young as 18 can rent one of these bikes, I definitely expected to see the dataset to have a much stronger right skew. While a right skew does exist, isn't extreme given that people in their 30's tend to ride more often than people in their 20's or even in their teens.

-In all gender types, the age range of 10-20 has the longest trip duration, this is maybe due to the young age still has more stamina, so they tend to ride the bikes longer either for recreation or for school, except for males which all age groups are nearly the same.