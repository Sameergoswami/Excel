**Renamed Initial worksheet name to Main. This holds main data source for all other calulations and other sheets. Made the following changes in the Main sheet.**

1. Conditional formatted to fill each cell in the `state` column with a different color, depending on whether the associated campaign was successful, failed, or canceled, or is currently live.
2. Created a new column O called `Percent Funded` that uses a formula to uncover how much money a campaign made to reach its initial goal.
3. Used conditional formatting to fill each cell in the `Percent Funded` column using a three-color scale. The scale should start at 0 and be a dark shade of red, transitioning to green at 100, and blue at 200.
4. Created a new column P called `Average Donation` that uses a formula to uncover how much each backer for the project paid on average.
5. Created two new columns, one called `Category` at Q and another called `Sub-Category` at R, by using **text to columns formula**.
6. Formatted Colums Q, R and I by making first letter capital by using **=Proper() formula** to make the data reading more appealing. Deleated original Q, R and I columns to avoid duplication.
7. Hide the original merged Category and Sub-Category column
8. Created a new column named at end `Date Created`to convert the data contained within `launched_at` into Excel's date format.
9. Create a new column named end `Date Ended`to convert the data contained within `deadline` into Excel's date format.

**Created a new sheet, Funding State By Main Category**, 
1. Created a pivot table that analyzes **Main** worksheet to count how many campaigns were successful, failed, canceled, or are currently live per **category**.
2. Create a stacked column pivot chart that can be filtered by country based on the table you have created.

**Created a new sheet, Funding State By Sub Category**, 
1. Created a pivot table that analyzes Main sheet to count how many campaigns were successful, failed, or canceled, or are currently live per **sub-category**.
2. Created a stacked column pivot chart that can be filtered by country and parent-category based on the table created.

 
  ![Outcomes Based on Launch Date](Images/LaunchDateOutcomes.png)

  * Create a new sheet with a pivot table with a column of `state`, rows of `Date Created Conversion`, values based on the count of `state`, and filters based on `parent category` and `Years`.

  * Now create a pivot chart line graph that visualizes this new table.

* Create a report in Microsoft Word and answer the following questions.

1. Given the provided data, what are three conclusions we can draw about Kickstarter campaigns?
2. What are some limitations of this dataset?
3. What are some other possible tables and/or graphs that we could create?

## Bonus

* Create a new sheet with 8 columns:

  * `Goal`
  * `Number Successful`
  * `Number Failed`
  * `Number Canceled`
  * `Total Projects`
  * `Percentage Successful`
  * `Percentage Failed`
  * `Percentage Canceled`

* In the `Goal` column, create 12 rows with the following headers:

  * Less than 1000
  * 1000 to 4999
  * 5000 to 9999
  * 10000 to 14999
  * 15000 to 19999
  * 20000 to 24999
  * 25000 to 29999
  * 30000 to 34999
  * 35000 to 39999
  * 40000 to 44999
  * 45000 to 49999
  * Greater than or equal to 50000

  ![Goal Outcomes](Images/GoalOutcomes.png)

* Using the `COUNTIFS()` formula, count how many successful, failed, and canceled projects were created with goals within the ranges listed above. Populate the `Number Successful`, `Number Failed`, and `Number Canceled` columns with this data.

* Add up each of the values in the `Number Successful`, `Number Failed`, and `Number Canceled` columns to populate the `Total Projects` column. Then, using a mathematical formula, find the percentage of projects that were successful, failed, or canceled per goal range.

* Create a line chart that graphs the relationship between a goal's amount and its chances at success, failure, or cancellation.

## Bonus Statistical Analysis

If one were to describe a successful crowdfunding campaign, most people would use the number of campaign backers as a metric of success. One of the most efficient ways that data scientists characterize a quantitative metric, such as the number of campaign backers, is by creating a summary statistics table.

For those looking for an additional challenge, you will evaluate the number of backers of successful and unsuccessful campaigns by creating **your own** summary statistics table.

* Create a new worksheet in your workbook, and create a column each for the number of backers of successful campaigns and unsuccessful campaigns.

  ![Images/backers01.png](Images/backers01.png)

* Use Excel to evaluate the following for successful campaigns, and then for unsuccessful campaigns:

  * The mean number of backers.

  * The median number of backers.

  * The minimum number of backers.

  * The maximum number of backers.

  * The variance of the number of backers.

  * The standard deviation of the number of backers.

* Use your data to determine whether the mean or the median summarizes the data more meaningfully.

* Use your data to determine if there is more variability with successful or unsuccessful campaigns. Does this make sense? Why or why not?
