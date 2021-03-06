# DAND_Project_6_Data_Vis
Udacity Data Analyst Nanodegree - Project 6 - Make Effective Data Visualization

## Summary
In this visualization, I would like to discover if there is any relationship between the height of baseball players and their batting average. The dataset contains 1,157 baseball players including their handedness (right or left handed), height (in inches), weight (in pounds), batting average, and home runs.

## Design
In the beginning, I decided to use bar charts with "height (in inches)" on the x-axis and "batting average" on the y-axis. I used only one color for the bars because I would like to avoid distraction from the colors. For each bar, I grouped up the data with the same height and calculated the average of the batting average in the group to represent the height of the bar. The graph shows that the batting average peaks at height of 67 inches and then slowly decreases as the height increases, except that there is a small jump at height of 79 inches.

After getting the first feedback, I added "handedness" to the category such that in each height group, we have three different bars showing the batting average for players using both hands, left hands, and right hands. To let readers spot the trends of different handedness more easily, I used three different colors to represent the three types of handedness. Surprisingly, there are no left handed players in the height groups of 65, 66, 78, and 80 inches, and there are no right handed players in the height group of 79 inches. The small jump in batting average at height of 79 inches is contributed by left handed players alone. Although the general batting average trends remain more or less the same, I noticed that left handed or both handed players have higher batting average than right handed.

After getting the second feedback, I tried to incorporate the number of players in each group to the graph. Hence, I stopped using bars, but bubbles to represent each group. It is because I can then use the size of the bubbles to represent the number of players. After using bubbles in the graph, I found that there are actually left-handed players in height 78 and 80 inches group, and right-handed players in height 79 inches. They could not been shown in the bar chart because they have batting average of zero. And we can see that the small jump in height 79 inches group is driven by one outlier left-handed player. In general, there are more right-handed players than left-handed, and more left-handed than both hands. It is also true for different handedness that the batting average in general trends downwards as the height increases, except that some outliers happened among tall players. Also, in general the batting average for left-handed and both hands players are higher than right-handed players.

After gettting the third feedback, I tried to add another series for the Home Run for each heights group. Similar to the batting average, I find the average of the Home Run for each group. Instead of using bar chart, I used line chart so that it won't obscure the bubble chart. The trend for the Home Run average is interesting. It doesn't follow the batting average exactly. It has a peak at height 67 inches, which means players in that group have both high batting average and Home Runs. However, it is not the same case for height 65 and 66 inches, where players have high batting average but not high Home Runs. In general, the trends for Home Run is not so clear, and I assume that is driven by other factors than height.

After getting the fourth feedback, I made some amendments to the windowsize, the tooltips, the legend labels, and the title. Also, I tried to add the total number of players in each Height group for the Home Run series. I added that information in bubbles form, and to avoid confusion with the bubbles in the Batting Average series, I turned the fill for Home Run bubbles to transparent. Not surprisingly, the area of the Home Run bubles should be the sum of the three bubbles for the Batting Average series. 

## Feedback
**Feedback 1**

It will be interesting to see the trends of the players in each height category further grouped by handedness.

**Feedback 2**

The graph doesn't show how many players are in each height group. The outliers in the trend may be driven by a small number of players.

**Feeback 3**

Can we also know the trend of the average of the Home Run among different heights groups?

**Feeback 4**

Below are some feedbacks from Udacity Project Reviewer:

1. Set the window size such that the chart auto fits the browser.

2. Rename the information in the tooltips such that it is more comprehensible for the reader, e.g. "avg" becomes "batting average".

3. Rename the legend labels, e.g. "L" becomes "Left-Handed".

4. Place the title closer to the chart.

5. Add the number of players (as bubbles) in each Height group for the Home Run series.

## Resources
[Dimplejs official site](http://dimplejs.org/)
