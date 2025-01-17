# Sales-Insights-Bricks-Mortar-Business-POWER-BI-SQL-
Designed a Power BI dashboard to understand AtliQ hardware goods sales trend. 

PURPOSE:

 To unlock sales Insights that are not visible before for sales team for Decision support & automate them to reduced Manual time Spent in data gathering.
 
PROJECT DESCRIPTION: 

 Designed a Power BI dashboard to understand AtliQ hardware goods sales trend. 
The final dashboard was effective at displaying the sales trend of AtliQ hardware, allowing users to understand the data and make informed decisions.
 This dashboard could help in increasing the revenue at least by 7% in the next quarter.
Sales team able to take better decision & prove 10% cost savings of total spend.
Sales Analyst stop data gathering manually in order to save 20% of there’re Business time and reinvest it value added activity.  

Key learnings:

   Connecting to Different data Sources.
 
   Data Transformation ETL In Power Query Editor and ETL processes for clean, reliable data.
 
   Creating Metrics using DAX & Data Modelling and Built data models for deeper analysis.
 
   Creating Data Visualization and Dashboarding
 
   Publishing to power BI Service. 

Sales Reports

https://app.powerbi.com/groups/me/reports/12de6c11-4f55-42a0-8675-9088d9b1f94b/d032985ec1c1fb1ca876?experience=power-bi
https://app.powerbi.com/groups/me/reports/12de6c11-4f55-42a0-8675-9088d9b1f94b/e5dfbe042bacaa84ce3f?experience=power-bi
https://app.powerbi.com/groups/me/reports/12de6c11-4f55-42a0-8675-9088d9b1f94b/253aef25e2d2a79fc3a3?experience=power-bi
https://app.powerbi.com/groups/me/reports/12de6c11-4f55-42a0-8675-9088d9b1f94b/a2bf66dd202192360bbb?experience=power-bi

https://github.com/Suraj-Boddhul/Sales-Insights-Bricks-Mortar-Business-POWER-BI-SQL-/blob/main/sales_insights%20PowerBI%20Feedback%20Improvement.pdf

https://github.com/Suraj-Boddhul/Sales-Insights-Bricks-Mortar-Business-POWER-BI-SQL-/blob/main/sales_insights%20PowerBI%20Feedback%20Improvement.pbix


Conclusion:

  This project underscores the significance of data analytics in enhancing business performance. By leveraging Power BI advanced features,the project not only provided valuable insights but also demonstrated how data can be a catalyst for growth and innovation.

Driving Future Success:

  I am excited to apply these insights and skills to future projects, driving continued growth and success.

Thank you for reading.😊


#






#
Sales Insights MySQL Query


Select * from sales.customers;

select cost_price from sales.transactions;

Select * from sales.products;

Select * from sales.markets;

Select * from sales.transactions;

select count(*) from sales.transactions;

Select Count(*) from sales.customers;

Select * from sales.transactions limit 6;

select * from sales.transactions where market_code="Mark001";

select count(*) from sales.transactions where market_code="Mark001";

Select * from sales.transactions where currency="USD";

Select Count(*) from sales.transactions where currency="USD";

Select * from sales.date where sales.date.year="2020";

Select sales.transactions.*, sales.date.* from  sales.transactions inner join sales.date on sales.transaction.order_date=sales.date.date where sales.date.year="2020";


select sum(sales.transactions.sales_amount) from sales.transactions inner join sales.date on sales.transactions.order_date=sales.date.date where sales.date.year="2020";

select sum(sales.transactions.sales_amount) from sales.transactions inner join sales.date on sales.transactions.order_date=sales.date.date where sales.date.year="2020" and market_code="Mark005";


select distinct product_code from sales.transactions where market_code="Mark001";
Select * from sales.transactions where sales_amount<=0;


Select distinct(transactions.currency) from  sales.transactions;

'INR'

'INR\r'

Select Count(*)  from  transactions Where transactions.currency='INR\r';

Select Count(*)  from  transactions Where transactions.currency='INR';

Select Count(*)  from  transactions Where transactions.currency='USD\r' or transactions.currency='USD' ;

Select *  from  transactions Where transactions.currency='USD\r' or transactions.currency='USD' ;

select sum(transactions.sales_amount) from transactions inner join date on transactions.order_date=date.date where date.year=2019 and transactions.currency="INR\r" or transactions.currency="USD\r";


select sum(transactions.sales_amount) from transactions inner join date on transactions.order_date=date.date where date.year=2020 and date.month_name="January" and  transactions.currency="INR\r" or transactions.currency="USD\r";


select sum(transactions.sales_amount) from transactions inner join date on transactions.order_date=date.date where date.year=2020 and    market_code="Mark001";


select sum(transactions.sales_qty) from transactions inner join date on transactions.order_date=date.date where date.year=2020 and    market_code="Mark001";
