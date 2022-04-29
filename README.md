# Kickstarter Campaign
Using Excel to uncover trends in the funding of theater productions

![Legend_Georgia](https://user-images.githubusercontent.com/30667001/164545434-5ccbd7a1-ac90-4c70-9a33-15289b796b68.png)

## Overview of Project
Playwright Louise wants to start a crowdfunding campaign to finance her theater production of *Fever*. With an estimated budget of $10,000, she is relying on results from this analysis to determine the factors necessary for achieving her fundraising objective. The crowdfunding data help to determine the best time and dollar range to maximize Louise’s success in realizing her financial goals.


On initial review, the Excel spreadsheet consisted of 4,113 rows of data and 14 categories. The following categories were of specific interest in this analysis:
|     Field                         |     Definition                                                                                                                                                                                                |
|-----------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|     goal                          |     Financial   goal to be achieved (dollars)                                                                                                                                                                 |
|     pledged                       |     Amount   provided by donors (dollars)                                                                                                                                                                     |
|     outcomes                      |     Categorical   result of campaign (successful, live, failed, canceled)                                                                                                                                     |
|     country                       |     Origin   of request                                                                                                                                                                                       |
|     currency                      |     Legal   tender of the request                                                                                                                                                                             |
|     deadline                      |     Start   of fundraising project (timestamp)                                                                                                                                                                |
|     launched   at                 |     End   of the fundraising project (timestamp)                                                                                                                                                              |
|     backers_count                 |     Number   of backers making a pledge                                                                                                                                                                       |
|     Category   and Subcategory    |     A   combined list of 10 project classes with secondary topics of variable   numbers; for the purpose of this analysis, the category of interest is   theater, and the subcategory “plays” specifically    |

From the data additional categories were creating including:
* The types of funded endeavors.
* Conversion of time to more useful formats.
* Percent of funding achieved.
* Average donations.

Two main questions came into focus:
1.	What were the outcomes for all theater funding requests, based on request launch date?
2.	What were the outcomes based on the financial goals of the requestor?

# Results
To answer the first question, a pivot table was created to analyze outcomes by month of the funding launch date. Live plays were not included in the analysis. Data were filtered by the parent category of theater. All years were included but limited to monthly display. Outcomes were sorted in descending order. From this data, a line chart was created to visualize the relationship between outcomes and launch month.

 ![Alt text](https://user-images.githubusercontent.com/30667001/146864450-d0a0a41e-17f3-4e6a-ac97-81154cf46344.png)

The next step was to determine outcomes based on financial goals. A table was created using the COUNTIFS() function. Continuous data were placed in categories by amount contributed. The number of successful, failed and canceled plays per monetary division was imported from the main spreadsheet. The percentage of successful, failed and canceled plays was then calculated based on these numbers.

 Based on populated data, a second graph was created to demonstrate the change in percentage of successful and failed goals, based on the amount of money requested.
 (*Note: Data not shown for canceled as no data to present.*)
 
 ![Alt text](https://user-images.githubusercontent.com/30667001/147697646-f7dd696a-a62f-4c1f-af84-b702af949af7.png)

 ### Analysis of Outcomes Based on Launch Date
Based on eight years’ worth of data, there are two conclusions about the Theater Outcomes by Launch Date:
1.	May appears to be the best month for a campaign launch for funding of theater plays as these campaigns are most successful when initiated in May.
2.	Campaigns launched in December appear to succeed and fail at almost equal frequency.

### Analysis of Outcomes Based on Goals
From the data around Outcomes Based on Goals, the greatest number of successful campaigns for funding plays are based on goals between $1K and $4,999. Goals below $5K are funded approximately 75% of the time. By comparison, funding of campaigns with goals of $10K falls to a rate of almost 50/50 when comparing success to fail.

### Challenges and Difficulties Encountered
•	The currency is listed in dollar amounts, but it is unknown if the conversion from one type of currency has occurred prior to spreadsheet publication. With 63% of the plays being US-based and 29% from Great Britain, it is the difference between these two countries that bears the most examination. As 1£ is currently equivalent to $1.31 US dollars, adjustments should be considered before this analysis is finalized.

•	When looking at data on plays specifically, the most data come from 2014-2017, with over 175 campaigns running each year and having an average success rate of 61%. Both before and after, however, fewer than 11 campaigns ran. It could be that there is something specific about that timeframe that could affect the interpretation of results based on the three years alone.

### Additional considerations could include a review of:
•	Timing associated with the campaign, such as Theater Outcome by Campaign Length, which demonstrates improved success when the campaigns run for fewer than 30 days (75% succeed). Running the campaign for two months, however, leads to an inversion, with 75% of campaigns failing from the two-month period onward.
 
•	Outcomes by number of donors. For instance, when limited to plays funded in the United States, the great majority were successfully funded when 20 individuals or more contributed to the campaign.

![Alt text](https://user-images.githubusercontent.com/30667001/146866001-d54e32e9-2cdd-46c6-9cfc-541ed34332e8.png)
  
