
# Ford Gobike System Data Exploration

## Dataset

The dataset consists of 519700 trip records from Bay Wheel in 2017. It could be downloaded from FordGoBike website (https://www.lyft.com/bikes/bay-wheels/system-data) by selecting the dataset of desired periode. 

## Summary of Findings

In the exploration, I observed an positive correlation on scatter plot between duration and distance (especially for the distance range of 0.5-3.5km) after transforming duration values in log. Besides, duration varies depending on user types and weekdays:  duration is longer in customer group than in subscriber, with small fluctuations across weekdays and slight increase on weekend. With a closer look at duration in the range of 500-2000 seconds and distance of trips under 8km, the difference in duration between groups remain consistant, whichever the day of the week.

Outside of the main variables of interest, I verified the relationship of distance variable to user type and weekday variables and found out that the distance made during trips on weekdays is generally longer than that on weekdend, despite of an opposite trend observed in duration-variable analysis. It suggests that the average speed of trips is very likely to be higher on weekdays than on weekend. <br>


## Key insights for presentation

For the presentation, I introduced firstly univariate distributions of four attributes of my interest by hist plot.<br> 

Secondly, I presented bivariate distribution between main variable duration and three others: distance, user type and weekday, relatively by a log transformed scatterplot, a boxplot and a violinplot.<br>

Thirdly, I displayed multivariate distribution of duration across user type and weekday, with a clustered boxplot. The original plot shows clearly difference across groups on weekdays but it's bit hard to interprete duration evolution across weekdays within one specific group. I further included a pointplot for a selected duration range of 500-2000 seconds to observe the trend that has been hidden on boxplot. <br>

In the end, I put an extra multivariate distribution with pointplot for the relationship of distance to user type and weekday to complete main findings for those who are willing to discover more about this bike trip dataset.  

## Reference
#### exploratory analysis:
- get the value of weekdays
from https://stackoverflow.com/questions/29096381/num-day-to-name-day-with-pandas
- calculate distance value between start point and end point with latitude and longitude
from https://gist.github.com/rochacbruno/2883505
