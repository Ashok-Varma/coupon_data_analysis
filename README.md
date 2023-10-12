# Analysis of Coupons Dataset
This data comes to us from the UCI Machine Learning repository and was collected via a survey on Amazon Mechanical Turk. The survey describes different driving scenarios including the destination, current time, weather, passenger, etc., and then ask the person whether he will accept the coupon if he is the driver. Answers that the user will drive there `right away` or `later before the coupon expires` are labeled as `Y = 1` and answers `no, I do not want the coupon` are labeled as `Y = 0`.  There are five different types of coupons -- less expensive restaurants (under \$20), coffee houses, carry out & take away, bar, and more expensive restaurants (\$20 - \$50).

## [Coffee House Coupons Analysis](coupon_analysis.ipynb#Analysis-on-Just-Coffee-House-coupons)

Analysed coupons for Coffee House and these are the observations from [the analysis](coupon_analysis.ipynb#Analysis-on-Just-Coffee-House-coupons)

1. [**Age**](coupon_analysis.ipynb#Age):

![Age to Acceptance](Images/Results/Coffee%20House%20Analysis/age_acceptance.png)

   - Individuals in the age groups 21-26 and 31-35 showed the highest acceptance rates. The youngest (below 21) and oldest (above 50) age groups had fewer instances of coupon acceptances.

2. [**Education**](coupon_analysis.ipynb#Education):

![Education to Acceptance](Images/Results/Coffee%20House%20Analysis/education_acceptance.png)

   - Individuals with "High School" and "Some College" education levels had a higher number of coupon acceptances. However, acceptance rates among those with "Bachelors" and "Graduate School" degrees were also notable.

3. [**Income**](coupon_analysis.ipynb#Income):

![Income to Acceptance](Images/Results/Coffee%20House%20Analysis/income_acceptance.png)

   - Acceptance rates were generally higher across most income groups, with especially high rates observed for those earning "Less than \$12,500" and between "\$50,000 - \$62,499".

4. [**Direction to Coffee House**](coupon_analysis.ipynb#Direction):

![Direction to Acceptance](Images/Results/Coffee%20House%20Analysis/direction_acceptance.png)

   - There was a higher acceptance rate for coupons when the direction to the coffee house was the same as the destination.

5. [**Time of Day**](coupon_analysis.ipynb#Time):

![Time to Acceptance](Images/Results/Coffee%20House%20Analysis/time_acceptance.png)

   - Acceptance rates peaked during late morning (around 10 AM) and again in the late evening (around 10 PM). Early morning hours like 6 AM saw lower acceptance.

6. [**Weather and Temperature**](coupon_analysis.ipynb#Temparture-and-Weather):

![Weather to Acceptance](Images/Results/Coffee%20House%20Analysis/weather_temp_acceptance_heatmap.png)

   - Across all weather conditions, there was a trend of higher acceptance rates at temperature extremes, suggesting that people might be more inclined to accept coffee coupons during very cold or warm weather.
   - Sunny days showed consistent acceptance rates across temperatures, with a slight peak at 80°F.
   - Rainy days had an upward trend in acceptance as temperatures rose, peaking at 80°F.
   - Snowy conditions saw the highest acceptance at 30°F, indicating a preference for warm beverages during cold weather.
   - Cloudy days, similar to rainy days, had increasing acceptance rates with rising temperatures, also peaking at 80°F.

### [Conclusion](coupon_analysis.ipynb#Conclusion):
- The temperature appeared to be a significant factor in influencing coffee coupon acceptance, regardless of the specific weather condition.
- People were generally more inclined to accept coffee coupons during times typically associated with coffee breaks: late morning, mid-afternoon, and late evening.
- Demographic factors such as age, education, and income also played a role in coupon acceptance.


## [Bar Coupons Analysis](coupon_analysis.ipynb#Investigating-the-Bar-Coupons)

Based on the observations and analyses conducted, we can hypothesize the following about drivers who accepted the bar coupons:

1. **Frequent Bar Visitors**: Drivers who frequently visit bars (more than once a month) are more likely to accept bar coupons. This makes intuitive sense, as those who already have a propensity for bar visits would find such coupons more appealing.

2. **Age Matters**: Younger drivers (under the age of 30) showed a higher acceptance rate for bar coupons compared to their older counterparts. This could be due to younger demographics being more social or more attracted to promotional offers.

3. **Presence of Children**: Drivers who had passengers that were not kids were more likely to accept bar coupons. This might indicate that drivers with kids are less likely to visit bars, possibly due to family commitments or the unsuitability of bars for children.

4. **Marital Status**: Those who were not widowed showed a higher tendency to accept bar coupons. While this might seem like a minor detail, marital status can often correlate with social behaviors and preferences.

5. **Occupation and Income**: Drivers who frequently visit cheaper restaurants and have a lower income (less than $50,000) were more likely to accept bar coupons. This suggests that economic factors play a role in coupon acceptance. Those with lower incomes might be more incentivized by discounts and offers.

6. **Specific Occupations**: Drivers not involved in farming, fishing, or forestry professions had a higher acceptance rate. While it's not immediately clear why this specific occupational group would be less inclined, it could be related to lifestyle, work hours, or regional factors.

In summary, drivers who are younger, frequently visit bars, are possibly more economically driven (given their inclination towards cheaper restaurant visits and income levels), and have specific lifestyle indicators (like not having kids as passengers or being non-widowed) seem to be more inclined to accept bar coupons.