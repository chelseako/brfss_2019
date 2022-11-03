# Diabetes and Health Care Access Data Visualizations and Analysis
2019 Behavioral Risk Factor Surveillance System (BRFSS)

## Code and Resources Used:
* R (ggplot2)
* Tableau

## Multi-Dimensional Scaling Average Number of Poor Health Days by State
![Multi-Dimensional Scaling](https://github.com/chelseako/brfss_2019/blob/main/MDS_State_Avg_Bad_Health_Days.png)
### Data processing and visualization
* Aggregated the BRFSS 2019 data by state and calculated the average number of:
    1. Bad mental health days
    2. Bad physical health days
    3. Days unable to complete daily living activities due to poor health
* Created multi-dimensional scaling coordinates and plotted using geom_point() and geom_label()
* Color coded labels according to region (West, Midwest, Northeast, South, Guam, and Puerto Rico)
* Shifted labels to avoid overlap

### Analysis
The visualization displays a cluster of southern states on the right side of the graph and a cluster of midwestern states on the left side of the graph, indicating that these states in close geographical proximity are also similar in terms of the overall health of their citizens as indicated by their average number of bad health days.  The Western and Northeastern states are clustered together in the middle of the graph, along with a few Midwestern and Southern states, and Guam. Certain states/territories are further away from any other states or clusters, such as West Virginia and Puerto Rico, indicating these states are different from the majority of the states in terms of their average number of bad health days.

## Choropleth - States' Percent with Health Insurance

![Percent with health insurance](https://github.com/chelseako/brfss_2019/blob/main/statePercentHealthInsurance2019.png)

### [Link to choropleth animation video](https://youtu.be/acC3c1pTr3k)
### Data processing and visualization
* Aggregated data and calculated states' percent with health insurance for each year from 2011 through 2019
* Joined tables to create and export single dataframe for use in Tableau
* Created the choropleth animation + interactive dashboard

### Analysis
The choropleth shows the states' percent with health insurance, with darker hues representing a higher percentage.  The animation displays the overall trend of percent with health insurance between 2011 through 2019 in the United States.  The states darken each year from 2011 through 2015, indicating a greater proportion of people have health insurance. In 2016, it appears that some states' percentages increased while others decreased compared to 2015. From 2017 through 2019, the U.S. overall becomes lighter, indicating a decreasing trend in the proportion of people with health insurance. 

## Dot Chart - Access to Health Care and Poor Health Days
![Access to health care inforgraphic](https://github.com/chelseako/brfss_2019/blob/main/healthCareAccess_infographic.png)
### Data processing and visualization
* Calculated average number of poor health days per month for those with and without the specified health care access
* Selected dot chart to minimize unnecessary ink
* Used symbols with legend to avoid crowded axis labeling
* Ensured chart and message were easy to understand for general public audience

### Analysis
The image shows that the greatest disparity in average number of poor health days between those with and without health care access is in mental health days, and the ability to afford care produces the greatest disparity in poor health days out of the four health care access variables.  Whether an individual had a checkup within the past 12 months produced the second greatest disparity.  Participants who did or did not report having a PCP did not differ on the number of poor physical health days and number of days unable to complete daily living activities due to poor health.  On average, individuals had approximately the same number of poor physical health days and number of days they were unable to complete activities, which was higher than the average number of poor mental health days.
