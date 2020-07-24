# When and Where do we bike in San Francisco? Ford GoBike Data Exploration
## by Maggie Kiraga

## Dataset

> In this investigation, I wanted to look at the characteristics of rental bikes' history from the San Fransico area to get some insights about characteristics that might influence the biking behavior. This dataset consists of 519,700 bike trips, spread over a period of approximately six months. The dataframe is made of 13 variables, where most of them are numeric in nature, providing information like rental location, duration, bike id, etc.

> The gathered data didn't require a lot of cleaning although I had to add some extra variables, like distance or weekdays, based on the existing ones. Later, I also changed the scale of the duration variable from seconds to hours, which easier the interpretation of the results. Also, I created a smaller subset of the most popular rental stations on which I performed the visualizations. 


## Summary of Findings

### Univariate numeric plots
> 1.Logarithmic distribution of the **duration** variable follows a normal distribution within which most of the rental time falls in the interval between 3 and 30 minutes, with a stepwise increase and the highest peak in the frequency when about 10 minutes.
2. **Distance** was an unimodal variable, with the peak values about 1 km, and long right-sided tail, where the distance of 5km and above are highly rare and its frequency almost invisible on the graph.
### Univariate categorical plots
3. When it comes to variable: **station name**, there is quite a big gap in popularity between the most and the least popular station from the ranking, especially so for the end stations, namely the most popular: San Francisco Caltrain was visited about 17,000 times when the number 10 from the ranking: Powell St BART Station, just about 9,000 times. Although those two stations are situated in close proximity to each other (1.5km), the former one lies next to the big train station, which might be sufficient enough to boost the popularity of the rental location. Another interesting fact is that three of the most popular start-renting stations are also the three most popular end-renting stations, although in a different order. 
2. Distribution of **weekdays** variable showed that the busiest days are Tuesday and Wednesday, being almost equally busy. Interestingly, the weekends are shown to be much less busy than the rest of the week, with Sunday's having the least number of customers. Another interesting observation is that the plots of start and end renting days look exactly the same, suggesting the same distribution of values.
### Bivariate findings
1. The station by the San Francisco Ferry Building showed to be most popular in almost all of the days. However, the differences between the 1st and 2nd most popular renting stations are quite small, this is in contrast to the third most popular station, which most of the time is only half as busy as the other two stations. Interesting is also the fact that all rental stations have a much higher number of customers on the weekdays (from Monday untill Friday) than at the weekends.
2. There was no relationship found between distance and duration variable. 
3. The rental time on the working days was quite similar and counted approximately 0.2 of 1 hour, meaning about 12 minutes. The mean rental time on weekends seems to be slightly higher and have a bigger variance of values. The statistics of the distance variable are very stable despite the day of the week, with a mean distance between stations slightly above 1 km mark. Both variables show long tails of systematically distributed, high values, although the scatter plot above showed that there is no correlation between duration and distance.
4. The duration variable is quite stable during the working days, and is approximately 15 minutes, whereas the average renting time on Sunday is slightly under half an hour. The distance variable is very evenly distributed during the week, with an average value of about 1.3 km.
### Multivariate results
1. Dividing the duration variable into two categories introduces more variability in the data and provides us with a more detailed view of the relationship between those two variables. We can see that Wednesdays have on average the longest duration time, contrary to the above findings which suggested that the longest duration time is on Sundays. This could be explained by the fact that, in general Wednesdays are much busier than Sundays, with a lot of rentals of short duration, which lowers the general average rental time on Wednesdays. Sundays on the other hand, might have generally less traffic, with a smaller number of short rentals, causing the misperception that the rental time on Sundays might be the longest.
2. There was a much higher number of rentals with low duration time and that there are fewer rentals on weekends than during the working days. Moreover, the distribution of the high rental time seems to be much equal during the whole week, with a much smaller variance than those rentals of low duration.


## Key Insights for Presentation

> 1. One main thread from when starting exploratory visualizations were large numbers of the extremely high values of the duration and distance variables. It helped to drop some of the outliers, as well as to narrow down the scale a bit. In the later section of the notebook, it proved to be useful to divide those two numeric variables into low and high categories of values, which helped to gain a better understanding of the data and the interactions between the variables.

