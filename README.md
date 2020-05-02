# Kickstarter Campaigns Analysis

## Project Overview
This module is a deep dive into Excel, a tool that can be used across all areas of life, from household budgeting to complex financial analysis. Learning the intricacies of Excel will draw on (and enhance) skills we may have already, like computer literacy, data literacy, and quantitative reasoning.
## Resources
Software: Excel

## Objectives
Use filters and Excel formula to create new datasets
Create visualizations using Excel charts and pivot tables
Interpret the summary data provided from the visualizations

## Summery of Challenge
We are given a data set from KickStarter campaigns for different categories and sub-categories. The data set includes many data columns, but we focus on the campaign start date, deadline, goal and the final outcome, in terms of number of campaigns (not the total pledged value)


## Descriptive Statistics for Successful and Failed Campaigns
Based on the data for successful and failed campaigns for plays in the US, the mean goal amount and pledged amount are higher than the median amounts, showing that the data is skewed. The standard deviations are also very large for each group of data.

## Musicals in Great Britain
The average goal amount for musicals in Great Britain is just over 4,000 GBP, shown by the x in the plot. This is much higher than pledged amounts without outliers. The median goal amount is 2,000 GBP, which is just over the upper quarter for pledged amounts. There is one outlier for each, shown by the dots, with a goal amount of 15,000 GBP and a pledged amount of 10,092 GBP.
## Recommendations for Louise
Based on the number of successful campaigns in theater, it would be reasonable for Louise to launch a Kickstarter for her play.

- The best time to launch would be in May.June or July are also good options.
- The goal amount of $12,000 for the play is an outlier for both goal and pledged amounts.Better to have a goal amount less than $6,000.
- The goal amount of 4,000 GBP for the musical is an outlier for both goal and pledged amounts. Better to have a goal amount less than 2,000 GBP.


### Outcome by Goal
First in the tab “Outcome Bsead on Goals”, I look at the data to determine whether the campaign goal contributes to its ultimate success or failure. I initially make 8 columns with headers of “Goal”, “Number Successful”, “Number Failed”, “Number Canceled”, “Total Projects”, “Percentage Successful”, “Percentage Failed”, “Percentage Canceled” on the sheet, made 12 new rows with specified group ranges and use Countif function in excel to calculate count of each column withing given goal range. Then on the “total Projects” column calculate total of each row using Excel’s “Sum” function. The percentage column consequently was calculated by deviding each of the first three columns and deviding it by the “Total Projects” column and multiplying it by 100. Finally a line graph was inserted to plot the count of each group versus the group range, for each of the first three columns. 
However I also use the “Lookup” function as a different approach instead of Countif on page “outcomes Based on Launch Goal2” to calculate count of all 12 ranges using pivot table which came up with the same result. 
The conclusion from this part of the challenge based on observation of the line plot for “Outcomes Based on Goal” is that the campaigns with goal of less $1000 has the highest chance of success and least chance of failure, while the campaigns with more than $50000 goal has the highest chance of failure and least chance of success. This is understandable that people would donate more to lower amount goals than higher. Interestingly there seems to be a local maximum in the success rate for the campaing with 40-45k goal. 
![Outcome by Goal](https://github.com/hbostanchi/Challenge-1-UCB/blob/master/outcome%20based%20on%20goal.png)
### Outcome by Launch Date
On the second part of the challenge, we were asked to look at the success rate of campaigns versus the launch date/month for “theater” categories. The results are on sheet  named “Outcome Based on Lunch Date”. First in the main table, I converted the launch date from Unix format to the mm/dd/yyyy format and then converted it to the month, in which the campaign was launched. Then I made pivot table on outcomes based on lunch months, which help us top look closer to the lunch time which played an important role on dentations. Based on the line chart observation the lunch date peaks on May and then steadily declines until September. 
![Outcome by Launch Date](https://github.com/hbostanchi/Challenge-1-UCB/blob/master/outcome%20based%20on%20Launch%20date.png)
### Outcome by Duration
Finally I also looked at the campaigns success rate depending on the duration of the campaign. First I calculated the targeted duration for each campaign by subtracting the launch date and deadline and converting it to number of days, in the main table. Then I generated a separate pivot table in tab “Outcomes Based on Duration” that shows campaigns with more than 70 days of duration have more than 85% of success rate.  
![Outcome by Duration](https://github.com/hbostanchi/Challenge-1-UCB/blob/master/outcome%20based%20on%20duration.png)
