# Kickstarting with Excel

## Overview of Project
The Data set have orgainized is use to help Louise analysis the decision making abount crowdfunding campaign project to help her theather play, names Fever that estimating the budget over $10000.

### Purpose
Generate table and graph to help Louise knows the different ampaigns will be fared by lunch dates and the funding goals, after Louise came close to its fundrasising goal         by providing the box plot and bar chart of the pivot table in same category of Louise's play Fever. 
## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
Creating a pivot table using count of outcomes as column value and every month of the year with "parent category-theater" and launch date "year" as the filter.
The line graoh was generated from this pivot table, Horizontal axis is month and horizontal axis is the number of outcome count. This graph can be provide Louise a visual summary of the data of pivot table, also uncovering a trend from the visualization. 

Before creating the pivot table, first we need to convert the unix timestamp into readable format to get the year of the launch date for the preparation.

### Analysis of Outcomes Based on Goals
In order to provide visualize line graph to Louise see the relation between outcomes and goals, first we need to create a table that state the percentage of each outcome in every $5000 goal range. Then the percentage that calculated by each kind of outcomes can be used as vertical axis in the line chart, the goal range will be the horizontal axis in the chart. 

The line graph above, clearly see a patern that outcome of successful and failed has the oposite trend with each other, and there are 3 intersect points. which can give Louise an idea about the balance funding goal amount for successful and failed.
### Challenges and Difficulties Encountered
During the problem solving stage, Challenges or diffulties are frequently occur in every project. In the analysis of outcomes Based on Goals, using the countifs() functionin EXCEL is the only challenge for me, since there are different when ranges are between 2 number compare to the range that only have 1 tail end. So I have went to google search and watched the hint to figure out the solution and overcome the challenge for using countifs() function in case that the range is between 2 numbers.  

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
From the Line charts of "Theater Outcomes by Launch Date", we can see that May and June are haveing the most successful outcomes in Theater category.
On the other hand, May to Aug almost have the same number of failed outcome, althought this are the months that number of outcomes were decreasing, number of 
successful are still higher than the number of failed and canceled. As conclusion the Theater category is the most successful one since haveing high successful 
outcomes and stable canceled outcomes in low number.

- What can you conclude about the Outcomes based on Goals?
From the Line chats of "Outcome Based on Goals Chart", we can see a patern that in the range less than $1000 to $24999 and range $40000 to $4999 are decreasing trend for percentage successful, increasing trend for percentage failed. In the range $25000 to $ $39999 and range $45000 to greater then 50000 are increasing trend for percentage successful, decreasing trend for percentage failed. Especially, the slpoe of line in range 30000 to 39999 and 40000 to 49999 are deeper then other. Also both successful and failed canceled remain unchange in range $35000 to $44999. percentage of failed and successful have the equal amount in range $15000 to$19999, $34999 to $39999. Therefore we can see that easy to success is the goals less then 1000, but wehn goal set to 25000 to 39999 will be increase the successful rate, especially the goal range 30000 to 39999.

- What are some limitations of this dataset?
The Kickstarter dataset we are workinng on has an error that we must correct it before start. In the Average Donation column there are #DIV/0! error occur, this error happen where the denominator of division formulac is 0. However not every campaign has backers, which make there is 0 as denuminator in the formula. Therefore we must clean the dataset before we go any further, in order to correct the error we use EXCEl iferror() function to debug. Since the eeor in dataset is kind of a missing values of the data, this could be consider as incomplete data and this could limit the usability of dataset. On the other hands, the dataset also have other limitation where using unix timestapm as format of date, this is the format that not readable until we need to convert the format by formula. 
- What are some other possible tables and/or graphs that we could create?
