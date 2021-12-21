# Module 1 Assignment - Kickstarting with Excel

## Background
After Louise’s play *Fever* failed to meet its fundraising goal, they contracted us to help her determine how they can succeed with future fundraising efforts. In particular, we were tasked with reviewing the success rates of Kickstarter campaigns based on two different factors related to the fundraising: launch dates and funding goals.

## Analysis and Results

### Analysis of Outcomes Based on Launch Date
The first thing that we wanted to review the data for is the impact that time of year has on the success of a campaign. We started by filtering the data to look at campaigns with the Parent Category of *Theater*. We then counted the number of campaigns by the month they started and the outcomes of the campaign (i.e., success, failed, and canceled). The resulting data can be seen in the line graph below.

![Theater Outcomes by Launch Month](https://github.com/kjminges/kickstarter-analysis/blob/main/Theater_Outcomes_vs_Launch.png)

Reviewing the data, May, June, and July are the months that produce the most successful campaigns. Unfortunately, when adding together the failed and canceled campaigns, these months also produce the highest number of failed and canceled campaigns.

In order to visualize the data better and account for the differences in the total count of the campaigns by month, we created the stacked bar chart below which shows the percentage splits for each month.

![Theater Outcome % by Launch Month](https://github.com/kjminges/kickstarter-analysis/blob/main/Theater_Outcomes_vs_Launch_2.png)

This data shows the percentage splits between successful campaigns and failed, or cancelled campaigns is pretty consistent throughout the year. For January through November, the success rate only varies by 10 percentage points (from 57% to 67%). The only real takeaway is that December is not a month which has shown success, with a success rate of 49%. The lack of success could be tied to the doners deciding to allocate their disposable income toward expenses that are typically associated with the holidays (travel, other donations, gifts, etc.).

We should be wary of the month-by-month data since it can be heavily impacted by the specific year. Take 2020 as an example. Q1 could be considered a "normal" year, but Q2 and Q3 would likely see a significantly high cancel rate and failure rate as COVID surged and states across the country locked down. As things started to open in Q4, and a large portion of the U.S. population had an abundance of monthly saved, they may have looked to donate more and help theaters that were adversely affected by COVID. This would lead to larger than normal donations and would skew data. 

### Analysis of Outcomes Based on Goals -
Next, we decided to look at the impact that the goal a campaign sets has on the overall success of the campaign. For this analysis, we were specifically looking at the campaigns with the Parent Category of *Theater* and the Sub-category of *plays*. We started by bucketing each campaign by their goal. The buckets start with $0 - $4,999 and increase by $5,000 increments for each subsequent bucket up to $50,000. The last bucket captures all campaigns with a goal of $50,000 or more. 

![Outcomes by Goal](https://github.com/kjminges/kickstarter-analysis/blob/main/Outcomes_vs_Goals.png)

Looking at the data it is clear that there are specific zones where plays tend to have a higher success rate. In particular, plays with goals less than $15,000 and between $35,000 and $45,000 have success rates around or above 55%. Looking closer at the numbers each bucket for Goals over $15,000 have less than 25 data points. This makes the data for the plays with higher Goals less credible when projecting the impact of setting a goal. That's why Louise should focus on setting a goal below $15,000. There is enough experience to consider the outcomes credible and the outcomes are more successful than not.

### Challenges and Difficulties Encountered

#### Data Limitations
- One limitation with the current data is the lack of detailed information regarding the payments that make up the total donations for each campaign. Especially for successful campaigns, the campaign could have been a success due to one or two large doners. This could be solved by adding an additional database with donation level data. The data could be tied back to each campaign using the campaign IDs in column A and would allow us to add statistical measurements like mean, median, standard deviation and variance to name a few. The statistics would give us more insight into how each campaign was funded and could allow us to remove outlier campaigns that may have been funded by one large doner. 
- For the purpose of Louise’s situation, it would also be advantageous to know which specific campaigns may be campaigns that have failed before. Adding a field that would allow us to investigate the specific campaigns that may have failed, and the changes that they made in order to make the campaign more successful.
- Finally, for some of the specific Parent Category and Sub-Category cuts, the data is not credible to make meaningful conclusions. More data will be needed to drive future actions.

#### Additional Analysis
After reviewing the data there are a couple other charts that we should be creating in order to perform a deeper review of the data for the purpose of Louise's. We already mentioned and provided the stacked bar chart for Outcomes Based on Launch Date. When looking at the success rate based on different variables, we need to make sure to consider the percent breakdown of the outcomes along with the raw numbers in order to effectively draw conclusions. We added the stacked bar chart to review the percentage splits and for the analysis of outcomes based on Goals, we should also look into providing a chart that shows the raw number of plays for each outcome. This will lead us to see how the data is skewed right and allow us to adjust our conclusions.

## Conclusion
Based on our analysis, it is hard to draw many conclusions for Louise regarding the time of year in which a campaign should begin, but we can advise that they avoid launching in December. With regards to the goal that Louise sets, they should try to keep it to smaller amounts, particularly below $15,000. This is where our data is more credible and where the success rate is favorable. These conclusions should be taken into consideration when beginning a new campaign in the future.
