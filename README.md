# PyBer_Analysis

## Overview of the analysis 
### Purpose: 
In the initial analysis performed on the ride share data, the percent of total rides, total fares, and total drivers by city type was calculated and visualized in scatter plots and pie charts. The purpose of this analysis is to take the same data that was used in our initial analysis a step further and provide a summary DataFrame of the Pyber ride-sharing data by city type and visualize the total weekly fares for each city type with a multiple line graph.  

## Results
The first deliverable of this analysis is the Summary DataFrame.  The analysis first calculated the total rides for each city type, the total drivers for each city type, and the total amount of fares for each city type.  Then the average fare per ride by city type and average fare per driver by city type was calculated.  These results were then put into the Summary DataFrame with the city type used as the index as shown below. 

![Summary_DataFrame](https://user-images.githubusercontent.com/103215123/170523705-63831d13-8ba7-4c5d-9a09-6d2cb26abb38.png)

For the second deliverable, a new DataFrame was created where the city type and date were set as the indices to show the total fares by date.  A pivot table was then created with the date set as the index and the columns were set as the city type, and the values in the pivot table was the fare data. The pivot table was then given a date range of 01-01-2019 - 04-29-2019: 

![fare_by_given_date_range](https://user-images.githubusercontent.com/103215123/170525698-e7c68bea-4713-4f3a-9e89-424e315ea69f.png)

A new DataFrame was created and the resample function was used to get the sum of the fares for each week.  

![resample_df_fares_by_week](https://user-images.githubusercontent.com/103215123/170526311-7ba48005-ac68-46d0-9465-9b4eb3c5e2c6.png)

The multiple line graph was then created from the total_fare_by_week DataFrame to give a visualization of of the total fares for each city type on a weekly basis. 

![PyBer_fare_summary](https://user-images.githubusercontent.com/103215123/170526660-a943bdbb-d4c2-4607-9baf-009e71ca694d.png)

## Summary
As might be expected, there is significantly higher amount of total fares in urban city types, 2 and 9 times more, than in suburban or rural city types respectively.  It should also be noted that in urban city types there are more total drivers, 2,405, than total rides, 1,625. Where as in suburban and rural city types there are more total rides than total drivers. This has an impact on the average fare per driver, $16.57/driver in urban cities vs $55.49/driver in rual cities.  This may have an affecct on or be indicative of the availability of PyBer rides in rural and suburban city types and show an opportunity to increase Pyber presence in these city types. Additionally, the mutiple line graph showing the total fares per week by city type shows that all three city types peak and valley in the same weeks, but the suburban and rural cities have flatter lines.  It would be beneficial to look closer at weeks that may have holidays and/or special events in urban areas and how Pyber may have the opportunity to better serve suburban and rural city types during these events.  
