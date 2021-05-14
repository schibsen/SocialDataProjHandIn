# Exploratory Data Analysis:



### Pedestrian volumes over the week:

A study of the pedestrian volumes over the week for different times of the day revealed that the volumes were more or less consistent for the different times of the day during weekends and weekdays except for day time. The day time volumes were almost halved indicating closed offices. An interesting pattern is also noted on Fridays: the volumes are similar from early morning through evening to those from Monday-Thursday. However, the late night volumes are almost twice as that of the other weekdays, which indicates that the area has a good night life. 

### Pedestrian volumes by hour of day:

As we explored the volumes based on the time of day across sensors we observed an overall shift of distribution towards the late hours on Fridays compared to Monday-Thursdays as weekend vibe sets in. Sensors could be picking up pedestrian activity generated for restaurant/club goers. Some sensors such as Bourke Street have moderate to high sensor volumes throughout the day; Lygon street shows high activity during the Friday late evenings whereas there are others that have high volumes during start of the business hours.


![test](Figures_interactive/boxplot_gif.gif)

We then created interactive visualizations to view the average pedestrian volumes by the hour based on the user's choice of a sensor and day of week. It helped us validate our observations from the boxplot. Further, it also pointed out which hour is the busiest or least busy in the day for each sensor, an information that isn't available through the Box plots. For example, the Bourke street sensors indeed show a drop in activity between 1pm-4pm , which then later picks up in the evening. Also, Princes Bridge and Southbank ( the names suggest proximity to a water body) pick up exceptionally high volumes around 5 pm which could also be driven by tourists.  

![test](Figures_interactive/bokeh_sensor_dayofweek_gif.gif)
