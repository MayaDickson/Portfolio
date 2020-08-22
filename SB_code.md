<a href="https://mayadickson.github.io/Portfolio/">Home</a>


# Super Bowl viewership and the ad industry over time
## Uses a line graph to compare three components
*Compares the average number of US viewers, household rating, and the ad cost for the Super Bowl over the years*

This is done by:
1. Creating a figure with a 3x1 subplot
2. Plotting the 3 subplots with the Super bowls as the x-axis
    1. Giving each subplot a title and a line color
    2. Sharing the x-axis label
3. Improving the spacing between the subplots


```python
plt.subplot(3, 1, 1)
plt.plot(tv['super_bowl'], tv['avg_us_viewers'], color='#648FFF')
plt.title('Average Number of US Viewers')

plt.subplot(3, 1, 2)
plt.plot(tv['super_bowl'], tv['rating_household'], color='#DC267E')
plt.title('Household Rating')

plt.subplot(3, 1, 3)
plt.plot(tv['super_bowl'], tv['ad_cost'], color='#FFB000')
plt.title('Ad Cost')
plt.xlabel('SUPER BOWL')

plt.tight_layout()
```
