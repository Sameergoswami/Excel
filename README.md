Files attahced
1.  `SG_Excel_HW_032021.xlsx`
      `Worksheets`
     `Main,Funding State By Main Category, Funding State By Sub Category, Project State By Yrs & Category, Bonus, Bonus- Statistical Analysis, Extar-     Funding Share`
2. `SG_Kictstarter_Campaign_Report_032021.doc`

**A. Worksheet `Main` holds the main data source for all other calulations and other sheets. Made the following changes in the Main sheet.**

1. Conditionally formatted to fill each cell in the `state` column with a different color, depending on whether the associated campaign was successful, failed, or canceled, or is currently live.
2. The new column O called `Percent Funded` that uses a formula to uncover how much money a campaign made to reach its initial goal.
3. Conditionally formatted to fill each cell in the `Percent Funded` column using a three-color scale. The scale should start at 0 and be a dark shade of red, transitioning to green at 100, and blue at 200.
4. The new column P called `Average Donation` uses a formula to uncover how much each backer for the project paid on average.
5.Created two new columns,`Category` at Q and `Sub-Category` at R, by using **text to columns formula** to split the signle column  `Category and Subcategory`.
6. Formatted Colums Q, R and I by making first letter capital by using **=Proper() formula** to make the data reading more appealing. Deleated original Q, R and I columns to avoid duplication.
7. Hide the original merged `Category and Subcategory`column
8. Created a new column named at end `Date Created`to convert the data contained within `launched_at` into Excel's date format.
9. Create a new column named end `Date Ended`to convert the data contained within `deadline` into Excel's date format.

**B. Worksheet `Funding State By Main Category`** 
1. Created a pivot table that analyzes `Main` worksheet data to count how many campaigns were successful, failed, canceled, or are currently live per **category**.
2. Create a stacked column pivot chart that can be filtered by country based on the table you have created.

**C. WorkSheet `Pivot Table Funding State By Sub Category`** 
1. Created a pivot table that analyzes `Main` worksheet data to count how many campaigns were successful, failed, or canceled, or are currently live per **sub-category**.
2. Created a stacked column pivot chart that can be filtered by country and parent-category based on the table created.

**D. Worksheet `Pivot Table Project State By Yrs & Category`** 
1. Created a pivot table that analyzesthat analyzes `Main` worksheet data how many campaigns were successful, failed, or canceled by categories and by years/months
2. Created a pivot chart line graph that visualizes this new table.

**E.  `Extra Work Done - Created a Pivot Table Funding Shares`**

**F. Created a report in `SG_Kictstarter_Campaign_Report_032021.doc` to answer the following questions.**
1. Given the provided data, what are three conclusions we can draw about Kickstarter campaigns?
2. What are some limitations of this dataset?
3. What are some other possible tables and/or graphs that we could create?

**G. The worksheet `Bonus` calculates the relationship between a goal's amount and its chances at success, failure, or cancellation**
1. Added 8 columns:**
* Goal
* Number Successful
* Number Failed
* Number Canceled
* Total Project
* Percentage Successful
* Percentage Failed
* Percentage Canceled

2. In the Goal column, created 12 rows with the following headers:**
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

3. Using the `COUNTIFS()`, counted how many successful, failed, and canceled projects were created with goals within the ranges listed above.

4. Added up each of the values in the  `Number Successful`, `Number Failed`, and `Number Canceled` columns to populate the `Total Projects` column. Then found the percentage of projects that were `Successful`, `Failed`, or `Canceled` per goal range.

5. Created a line chart that graphs the relationship between `A goal's amount and its chances at success, failure, or cancellation`.

**H. Statistical Analysis**
1. The worksheet `Bonus-Statistical Analysis` aims to understand whether the mean or the median summarize the data more meaningfully and to determine if there is more variability with successful or unsuccessful campaigns by comparing the Means, Medians, Min and Max, Variences, and Standard Deviations of Sucessful and Unsuccessful Campaigns .**

Feedback on the statistical analysis on whether the mean or the median summarizes the data more meaningfully and if there is more variability with successful or unsuccessful campaigns. Does that make sense? Why or why not? has registered in the attached word file  `SG_Kictstarter_Campaign_Report_032021`

