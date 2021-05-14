# Exploratory Data Analysis:



### Pedestrian volumes over the week:

A study of the pedestrian volumes over the week for different times of the day revealed that the volumes were more or less consistent for the different times of the day during weekends and weekdays except for day time. The day time volumes were almost halved indicating closed offices. An interesting pattern is also noted on Fridays: the volumes are similar from early morning through evening to those from Monday-Thursday. However, the late night volumes are almost twice as that of the other weekdays, which indicates that the area has a good night life. 

### Pedestrian volumes by hour of day:

As we explored the volumes based on the time of day across sensors we observed an overall shift of distribution towards the late hours on Fridays compared to Monday-Thursdays as weekend vibe sets in. Sensors could be picking up pedestrian activity generated for restaurant/club goers. Some sensors such as Bourke Street have moderate to high sensor volumes throughout the day; Lygon street shows high activity during the Friday late evenings whereas there are others that have high volumes during start of the business hours.


![test](https://github.com/schibsen/SocialDataProjHandIn/blob/0c26b6bbdf5e3f83c06788e5137ac4757d8fcf8e/Figures_static/boxplot_gif.gif)

We then created interactive visualizations to view the average pedestrian volumes by the hour based on the user's choice of a sensor and day of week. It helped us validate our observations from the boxplot. Further, it also pointed out which hour is the busiest or least busy in the day for each sensor, an information that isn't available through the Box plots. For example, the Bourke street sensors indeed show a drop in activity between 1pm-4pm , which then later picks up in the evening. Also, Princes Bridge and Southbank ( the names suggest proximity to a water body) pick up exceptionally high volumes around 5 pm which could also be driven by tourists.  

![test](https://github.com/schibsen/SocialDataProjHandIn/blob/0c26b6bbdf5e3f83c06788e5137ac4757d8fcf8e/Figures_static/bokeh_sensor_dayofweek_gif.gif)


### Weather
Imagine being in Melbourne right now, how do you think the weather would be right now? And would that somehow influence the local peoples social behaviour ? Would it be possible to predict how many people are walking on the streets based on day time and weather?  Those are some of the questions we asked ourselves, because you see in the Nordic countries people are very influenced by the weather, a cold and rainy is better spend idoors with a nice cop of coffe and a good book.   

Therefore we inspected the weather in Melbourne for the period 2018-2019, and compared it with the Pedestrian data of Melbourne. 
The weather variables that we had acces to which are easy to understand are Temperature, relative Humidity and Windspeed, thus lets take a close look on these 

![weather variables](Figures_static/weather_plot.png)

The plot shows us that the temperature is dependant on the season, whereas relative humidity and wind speed has no seasonal pattern 
Air temperature follows a skew normal distribution. The same holds for Windspeed even though it is not as clear as for the temperature.   
However relative humidity does not follow a noral distribution since many observations show a relative humidity around 100% . 


### Weather and social behaviour

We looked at the relation between weather and pedestrian flow, and found two very interesting sensors mirroring social behaviour based on weather, so let's dive into that. The two sensors we are going to look at are *Southbank* and *Lygon St (West)*, the location of the two are shown below

![sensor locations](Figures_static/2focus_sensors.png)

We decided to look at the pedestrian flow between the hours 6 and 22 as this is were most people are on the streets. 





The plot below shows pedestrian counts for the sensor at southbank for four selected timeslots alongside the mean temperatures. There is clearly a positive corelation, meaning that there are more pedestrians when the temperatures are higher. This patterns are more profount in the mornings and late evening, whereas the coreation is more noisy in weekends and evening rush hours. One could hypothesice that decision regarding the mean of transportation to and from work for those who have the choice, is made in the mornings. In the afternoon, you are stuck with or without the car you took in the morning. In the evening once again you are free to go out, if the weather is attractive. For the weekends the months of July and November are deviating from the general picture, in opposite directions, that coule be worth looking further into. In July some activities, which do not take place during the other summer months, seem to be attrcting people to the streets on weekends. Melbourners might be instantly aware, what this is, but as data travellers, we can only conclude that we have stumpled across something we can't explain, and would like to look further into, possibly by including other sources of data. 




![southbank](Figures_static/southbank_weather.png)


In Lygon st. (west) the patterns are wery different for different times, during the week. In morning rush hurs we see a tendency, similar to that of Southback, where higher temperatures coinside with higher numbers of pedestrians. This pattern is also to some extent pesent fo the evening rush hours as well as for the weekend, but this pattern is only distinguashable because there are visibly fewer pedestrians in the winter season - is does not old for comparing two summer months to each other. Perhaps most curously, the morning volumes seem to follow a completely different logic. The pedestrian volumes passing the sensor at Lygon st (west) in the mornings  maintain similar levels through the months February-November. However, in december and January, the levels drops very visibly. A tendency wich does not exist for the other time slot, nor can it be explained by the temperatures. 




![southbank](Figures_static/lygon_weather.png)
