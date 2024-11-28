**Bike Store Sales Analysis Report**

**Product Overview:** This data shows the amount of sales done in a bike store from the year 2013 to 2016. It contains the Date, Day, Month, Year, Customer_Age, Age_Group, Customer_Gender, Country, State, Product_Category, Sub_Category, Product, Order_Quantity, Unit_Cost, Unit_Price, Profit, Cost and Revenue. The data comes in a csv file

**Link to dataset:** https://www.kaggle.com/datasets/prepinstaprime/europe-bike-store-sales

**Dataset Description:**
•	Date: Date of purchase from 1st January 2011 to 31st July 2016
•	Day:  The Day of Purchase eg 1st
•	Month: The Month
•	Year: Purchase Year
•	Customer_Age: The age of a Customer_ranges from 17 to 87
•	Age_Group: Displays the age group based on the customer age Youth (<25)
•	Customer_Gender: Gender type of Customers, M for Male, F for Female
•	Country: Countries where the bike stores are located
•	State: States from the country by which the stores are at
•	Product_Category: Category of products from Accessories, Clothing and Bikes
•	Sub_Category: These are the products under the category example are bikes racks, caps, cleansers etc
•	Product: The products here are different type of variations of the sub category products
•	Order_Quantity: This is the amount of quantity a customer ordered a certain product
•	Unit_Cost: $, the unit cost of a single product 
•	Unit_Price: $ the unit price of a single product
•	Profit: $ the profit gained after removing the cost from the revenue
•	Cost: $ unit cost multiplied by the quantity
•	Revenue: $ unit price multiplied by the quantity

**Problem Statement:** The following are challenges, questions or issues the company may face or experience from this dataset:
1.	Wrong values in the Cost and Revenue Columns: From this dataset it is seen that the values in the Cost and Revenue Columns are quite wrong. There is a miscalculation of cost and revenue values which will lead to a bad record or analysis and even produce wrong prediction of sales for the next 5 to 10 years. Aside from that, since both the revenue and the cost values are wrong, this means therefore that the profit value and every other calculation done like marginal percentage, revenue percentage, etc will be incorrect as well.

2.	 Identifying key metrics: The bike stores are constantly visited as a lot of customers are in need of their products, the managers, directors etc are trying to understand their     customers choices and preferences on their products, over the years based on the customers gender or age groups in different states and countries at which the stores are located. This analysis provides insights, trends that will be used to make data-driven decisions to enhance and grant the stores great profit and revenue for the future.

**Data Analysis Tools:** For this dataset, two analytical tools were used, they are:
•	SQL SERVER MANAGEMNET STUDIO (SSMS): This tool was used for data cleaning, data manipulation, data exploration, transformation and deep analysis
•	Power Bi: This tool was used for data visualizations and dashboard creation showing all insights and trends through the dashboards

**Research Questions:** These are the following questions used on the focus on uncovering trends, insights and patterns
1.	What are the sales trends over the years?
2.	Which country has the highest revenue?
3.	Which state has the highest sales?
4.	Which gender produced the best sales in the store
5.	How does the age group (adult, young adult, senior and youth) affect the trends of the sales
6.	The top products ordered over the years
   
Analytical Dahshboard
![Dashboard](https://github.com/user-attachments/assets/85141b46-b779-4852-95b0-44a9ab80e76d)


**Analysis Steps
Data Cleaning and Transformation:** The following process took place for the transformation and cleaning of the sales data
1.	Removal of duplicates/null values: There were not any duplicates nor either blank/null values in the sales dataset as each row showing unique values.

2.	Splitting of Columns: On the sales table, the column Age_Group was split into two columns which are the 
a.	Age_Range: this displays the age range of cutomers ie (<25), (35-64) etc and 
b.	Age_Groups: this diplays the various customer age groups ie young adult, senior etc.


3.	Deleting Columns: Using the alter and drop column function, the age_group column and the date column was removed. The Age_Group which was originally in the dataset has been removed since we have both the Age_Groups and Age_Range columns. As for the Date column,  it was removed as there is already a day, month and year column

4.	Calculation of revenues, cost and profit: One of the key issues identified was the miscalculation of revenue, costs, and profits in the sales dataset. This was resolved by updating the table and ensuring accurate calculations for each column.

**Deep Analysis** on Key Metrics and Insights of the Sales Data: The process of deep analysis on the sales table was done using aggregate functions such as sum, count, avg to make calculations. The use of view functions and case functions were also used in the deep analysis.

**Visualizations and Interactive Dashboard: **
1.	Importing the cleaned and transformed data from sql server to power bi desktop
2.	Loading the data to the model
3.	Use of charts such as line graph, bar charts, doughnut charts for displaying of insights such as Revenue by Age Group
4.	Use of cards to display the metrics such as Total revenue, total quantity ordered etc….
5.	Use of slicers to filter through and ensure the dashboard/ reports are interactive

**INSIGHTS AND FINDINGS FOUND FROM THE ANALYIS**
1.	Metrics over the years: From the year 2011 to 2016 we obtained the following:
    a.	Total Revenue:  $95,176,318 or $95M
    b.	Total Quantity Sold: $1,345,316 or $1M
    c.	Total Profit: $42,126,410 or $42M
    d.	Avg Customer Age: 35

2.	Annual/Yearly Revenue and Profit: From the year 2011 to 2016, we noticed that the company made a lot of sales and acquired great profit in the year 2015 with a total revenue of   $22,405,052 and a profit of   $9,909,624. Also it is seen that there was a reduction in sales and profits after the year 2015. So in the year 2016, there was a great decrease of $2,723,283 from the revenue in the year 2015. It also seen that something like this occurred between the year 2013 and 2014 revenues. This situation also caused a great effect in the profit

3.	Customer Gender demographics: Over the years we see that there were more male customers than female in the bike stores having the values of the male customers to be 58,312 while for the female customers there are 54,724. Following this we see the revenue and revenue percentage by gender as
    a.	Male Gender Revenue: This is resulted to a total of $48.33M and a percentage of 50.78%.
  	The highest revenuefrom the male customers was in the year 2015 with a total of $11,149,645 and its percentage is 11.71%
  	
   b.	Female Gender Revenue: This is resulted to a total of $46.85M and a percentage of 49.22%. 
   The highest revenue from the female customers was in the year 2015 with a total of $11,225,407 and its percentage is 11.83% 

5.	Monthly Revenue and Profit: Over the years, the bike store made a lot of money sales and profit in the month of December with a revenue of   $10,158,080 and profit of   $44,80,861, while the company had a lower sales in the month of August with it revenue $6,348,349 and its lowest   profit was in the month of July with a total of   $2,810,336.

6.	Top Ordered/Sold Product (based on Sub_Category): From the analysis, the top 5 ordered products made by the store over the years was captured over the years. So therefore, the product by sub_category that has the highest order or sold is Tires and Tubes with a total of   514,051 quantity. While the Touring Bikes product had only 4648 quantity sold, which makes it the lowest product sold based on the top 5 list.

7.	Top Selling Countries: From the analysis, the top 5 countries with highest revenue was captured, marking United States as the no 1 Country that has the highest revenue worth of   $30,814,774 and the country with the lowest is France with a revenue worth $ 9,847,213

8.	Revenue by Age_Range: The analysis provided the revenue for the age range of customers over the years. They are as follows: 
Age Range	Total Revenue
      1.	(35-64):	47,323,876
      2.	(25-34):	34,310,905
      3.	(<25):	13,201,837
      4.	(64+):	339,700
From the above table we see that the age range with the highest revenue is ages (35-64) and the lowest is ages (64+).


**#Recommendation**
1.	Address Revenue Declines: Investigate factors contributing to the revenue drops between 2013-2014 and 2015-2016 to identify recurring patterns.  Implement strategies such as aggressive marketing, pricing adjustments, or product diversification to reverse these declines.

2.	Capitalize on Peak Performers: Focus on boosting sales for top-performing products like Tires and Tubes by increasing stock availability and marketing campaigns. Strengthen December promotions to maximize revenue during the most profitable month.

3.	Broaden Demographic Engagement: Maintain focus on the age group 35-64, which generates the highest revenue, while creating strategies to attract younger (<25) and older (64+) demographics for additional growth opportunities.

4.	Enhance Gender-Specific Marketing: With male and female revenue contributions nearly equal, tailor campaigns to address specific preferences and needs of both genders.
5.	Geographical Strategy: Expand efforts in top-performing regions like the United States to sustain dominance. Conduct further research into underperforming markets, such as France, to identify barriers and opportunities for growth.

6.	Seasonal Inventory Planning: Adjust inventory to meet increased demand in December while minimizing potential overstock during slower months like August and July.

**Conclusion**
The bike store demonstrated strong performance from 2011 to 2015, but the recurring revenue declines in subsequent years highlight the need for targeted interventions. By focusing on peak-performing products, demographics, and regions while addressing areas of underperformance, the company can stabilize growth and enhance profitability. These adjustments will ensure long-term resilience and market competitiveness.


