# Kickstarter-analysis
Performing analysis on kickstarter data to uncover trends
## Overview of Project

### Purpose
The purpose of the project was to use Excel to analyze kickstarter data to determine the success of fundraising goal for other campaigns in relation to their laucnch dates and their funding goals.  We used different formulas to sort the information in the dataset that was provided and then we used charts and tables to show visualization of the analysis that was done.
## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
In the analysis of the outcomes based on launch date (Deliverable 1) a pivot table was used to filter for parent category and for the year they started raising funds.  A new column was created in the kickstarter data set to show just the year out of the start date.  This was done by using the formual "=year(S2)" and filling down for the remaining values in the column. The columns of the table showed the outcomes of the campaigns showing successful, failed, canceled and the grand total.  The rows were filtered out to show the date created so that the months of the year are listed and the value showed a count of the each outcome displayed out for each month of the year.
### Analysis of Outcomes Based on Goals
In the analysis of the outcome based on goals (Deliverable 2) we set up a table determine the percentage of the successful, failed, and canceled plays based on the funding amount.  We first had to sort our the goal amounts for each category which started at the the amounts up to $1000 and ending at $50,000 and over.  The intervals in between went up in intervals of $5,000.  In order to sort the information we used "countifs" formulas.  
The countifs formula uses a range of data and filters based on a certain criteria being true and continue in that pattern checking for more criteria and will count how many meet all the requirements.  An example of the formula used to see how many plays successfully met their goal between $1,000 - $4,999 would look like this (=COUNTIFS(Kickstarter!$D$2:$D$4115, "<1000",Kickstarter!$F$2:$F$4115, "=successful", Kickstarter!$R$2:$R$4115,"=plays").  The Sum formula was  used to get totals for each interval amount between successful, failed and canceled outcomes, and then a percentage of each outcome was formulated for each interval.  The percentage was found by dividing the each of the three outcome by their respective grand totals.  The results were then presented on a line chart.

### Challenges and Difficulties Encountered
When going through the steps for Deliverable 1 there weren't any real issues that were experienced since it was pretty straight forward. The majority of the difficulties that were experienced were in Deliverable 2.  My primary issue was in getting the syntax correct to return an actual number value.  I was able to google the correct syntax to get the number values to display.  Once that was done it took a while to figure out that the data was off because i left out the part of the formula that had it look specifically at the plays category instead of all the categories listed in the dataset.
## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
One of the conclusions that i gathered from the data is that the successes out numbered the falures for the most part by a wide margin with very few campaigns that had to be canceled.  Another conclusion that was noticeable from the data was that the most successful months were May and June and by a very noticeable margin.
- What can you conclude about the Outcomes based on Goals?
One of the conclusions that i gathered from the data calculated is that for whatever reason there were absolutely no canceled fundraising campaigns in regards tot he plays in the data that was gathered.  Another noticeable conclusion from the data is that the the majority of the success were in the amounts that were approximately $5,000 or less, and that the once the goals were over $20,000 the failures overtook the successes.

- What are some limitations of this dataset?
There weren't any obvious limitations in the dataset.  The sample size seemed to be adequate and their wasn't any reason to think that the data wasn't reliable given that it was just hard data amounts instead of an oppinion pole for example which can have a variety of biases involved.
- What are some other possible tables and/or graphs that we could create?
For both of the deliverables using a clustered column bar graph would have been just as effective showing the results of the data that was gathered.  This would have been especially true for the results in deliverable 2. 
