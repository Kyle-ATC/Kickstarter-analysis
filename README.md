***Kickstarter-analysis***
- **Deliverable 1: Outcomes based on Launch Date Chart**
    - Year and Month for all projects Outcomes
      - Table 1
 ![This is an Image](https://drive.google.com/file/d/1LB-tu614VghtsqcTFG6CVh9UzthmPvaa/view?usp=sharing)












     - Theatre Outcomes based on months from 2009 to 2016
       - Table 2
 ![This is an Image](https://drive.google.com/file/d/1KnheDR1VaWD8SjgTQ7uE_g41_bODSzYG/view?usp=sharing)











    - US Theatre Plays in 2016 (i.e. Fever) 
      - Table 3
 ![This is an Image](https://drive.google.com/file/d/1i9fAOB3c3tryJPx5rt8TD3IttFn_ba5p/view?usp=sharing)











- **Deliverable 2: Outcomes Based on Goals Chart**  
    - Outcomes based on all calendar years
      - Table 4
 ![This is an Image](https://drive.google.com/file/d/16wxf2SjaEBadlaJtcFzHn6LL6Wxgk4aI/view?usp=sharing)










    - Outcomes based on goals in 2016
      - Table 5
 ![This is an Image](https://drive.google.com/file/d/16U9Ea99lMZrWerZrbItHSnhcRHkKivpB/view?usp=sharing)


**Deliverable 3: Written Analysis of the Results**
**Overview and Purpose**
The Kick Starter Program has reviewed several different productions for various forms of entertainment.  These various forms include but are not limited to board games, live theatre, movies, music, technology, food and various others. It has collected a wide range of data sets that can be helpful for future planning related to raising funds, goal setting, country, time of year and several internal factors related to each project.
The purpose of this Deliverable is to highlight what could be two Key Performance Indicators (KPI’s) when future projects are selected to A) start and their rate of being successful and B) success compared to the goal that was set for fundraising to initiate the project and the outcome for Louise.
This will be compared specific to the Play Fever by Louise that had 

1. 	A goal of $2,885 
2.	Raised $2,485 
    - 3.	Failed to meet its goal by 14%
4.	Started its fundraising in 6/13/2021
5.	Ended its fundraising on 7/11/2016
    - 6.	Was given 1 month to raise its required capitol (goal)

**Analysis and Challenge**
*Analysis*
Formula for deliverable 1
- =month()
- =year()
Formula for Deliverable 2
- =COUNTIFS(Kickstarter!$D:$D, "<1000", Kickstarter!$R:$R, "plays", Kickstarter!$F:$F, "Successful")
- =COUNTIFS(Kickstarter!$D:$D, "<1000", Kickstarter!$R:$R, "plays", Kickstarter!$F:$F, "Failed")
Table 6
![This is an Image](https://drive.google.com/file/d/1FCnYhVb3alrD-iARW6vUlhjgNerhXioV/view?usp=sharing)

*Data Formatting*
Most of the learning lessons were from recoding data into something more usable.  One of the biggest challenges in the first chart was to switch date into a Gregorian from Unix, a more user-friendly function.  I first attempted to switch this after creating the pivot table.  This taught me to have usable data first, then move the data to a new tab or table.  The Unix date was still the same when moved over, even though I had the formula for conversion. This meant, that even with the Gregorian format showing, it was still technically in Unix, not allowing to me to sort my months.

*Data Validation*
Another challenging part, which I have still yet to solve, is for the percentage of successful to failure for the Plays based on goals.  I was comparing a separate, but should have been the same value, formula from the kick starter tab for total Plays directly pulled from the kick starter sheet.  I was comparing this to the successful, failure, and canceled goals opposed to using the total numbers themselves from the three categories.  While the chart was usable, it was not valid as the total percentage did not equal a 100%.  This leaves questions that will be discussed in conclusion. The chart below (Table 7) illustrates the findings. Column C and Column D should have the same total Plays, even though different formulas were used. Examples for Row 4 (1000 to 4999 in Column A) are shown below.

-Column C

=COUNTIFS(Kickstarter!$D:$D,">=1000", Kickstarter!$D:$D,"<=4999", Kickstarter!$R:$R, "Plays")

-Column D

=COUNTIFS(Kickstarter!$D:$D,">=1000", Kickstarter!$D:$D,"<=4999", Kickstarter!$R:$R, "Plays", Kickstarter!$F:$F, "Successful")

=COUNTIFS(Kickstarter!$D:$D,">=1000", Kickstarter!$D:$D,"<=4999", Kickstarter!$R:$R, "Plays", Kickstarter!$F:$F, "Failed")

Table 7
 ![This is an Image](https://drive.google.com/file/d/1GEmNq7pCV7JOfR6e03QDQf37fWrN3RYR/view?usp=sharing)

**Conclusions/Results**
	*May is the Best Month*
The Chart “Theatre Outcomes based on months from 2009 to 2016” depicts all theatre outcomes by month over the course of 7 years. This entire time frame with and x axis of months, shows that, while May is the month that seems most likely to reach your fundraising goal, it is also the highest month for failed outcomes. Fever started its fundraising in June, which is show by the chart to be a good chance of success.  Unfortunately, the show fell 14% short of their desired outcome.
	*Total Fundraising Goal*
Fever had a goal of $2,885.  This falls into the subset of $1,000 to $4,999 which had a 73% success rate in reaching their goals across the 7-year span.  If we get even more specific/granular; 2016 had this subset have an even higher success rate of 76%. It would that Fever fell into the unfortunate category of failure despite having potentially very good metrics for success, but this data is still limited to draw that conclusion.

**Limitations**
*Only Factors Related to Theater Opposed to Target Population*
There are several factors that across several years.   The good is the data all seems very consistent.  We do not dive into year over year analysis to review yearly trends, but the total.  We also do not analyze to see how statistically relevant this data is.  A regression analysis would be helpful.
*Category and Subcategory*
When the first analysis for time of year and outcomes was conducted, it was asked to viewed as “Plays” in the subcategory of theatre.  The other analysis of outcomes was to be performed with “Theatre.”  This is difficult to draw comparison between the two as this now a category vs a sub-category
Should view goal amount in relation to the time frame to raise that goal

**Other Analysis**
*Specific to the Question and Population*
All analysis when looking for trends should be as specific as possible so that it is the most relevant information to your question of “how other campaigns fared in relation to their launch dates and their fundraising goals.” This is why in the beginning there are three (3) additional charts that were not asked for and that I also reference. This specificity, while not all that dissimilar, strengths the position of the analysis for Louise.
*Increase in more Kickstarter Projects*
In the first chart, it is viewed of every kickstarter fundraiser.  Over the years there are more and more fundraising programs. While failure always happened, programs started being canceled as well as a much larger increase (potentially) is seen in the failures of all programs.  More analysis is needed in this area to determine.
*Only 2016 Data*
There is an addition chart (Table 5) that I created to show that 2016 was an import graph to show. Most theatre productions in that year were labeled “failure” as they did not meet their desired fundraising goal.  Even though the year over year data would suggest Louise should have accomplished her fundraising goal (even within the 2016 year), they overall Theatre groups were not successful in this.  Table 5 is shown again below.

Table 5
![]()
