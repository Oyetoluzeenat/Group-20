parch_poseyData Analysis Project

Project Overview

This project involves exploratory data analysis (EDA) on sales and marketing data from a PostgreSQL database to derive actionable insights and recommendations. The analysis covers accounts, orders, sales representatives, regions, and web events.

Data Tables

The data is organized into five primary tables in the posey database:

Account
    id: Integer (Account ID)
    name: Varchar (Account Name)
    website: Varchar (Account Website)
    latitude: Numeric (Latitude)
    longitude: Numeric (Longitude)
    primary_poc: Varchar (Primary Point of Contact)
    sales_rep_id: Integer (Sales Representative ID)

Orders
    id: Integer (Order ID)
    account_id: Integer (Account ID)
    occurred_at: Timestamp (Order Date)
    standard_id: Varchar (Standard ID)
    gloss_qty: Integer (Gloss Quantity)
    poster_qty: Integer (Poster Quantity)
    total: Numeric (Total Amount)
    standard_amt_usd: Numeric (Standard Amount USD)
    gloss_amt_usd: Numeric (Gloss Amount USD)
    total_amt_usd: Numeric (Total Amount USD)

Region
    id: Integer (Region ID)
    name: Varchar (Region Name)

Sales_rep
    id: Integer (Sales Representative ID)
    name: Varchar (Sales Representative Name)
    region_id: Integer (Region ID)

Web-event
    id: Integer (Web Event ID)
    account_id: Integer (Account ID)
    occurred_at: Timestamp (Event Date)
    channel: Varchar (Web Event Channel)

Insights

Here are the key insights from the exploratory data analysis:

Total number of accounts: 351
Missing values: No missing values in key fields (name, website, primary_poc, latitude, longitude).
Sales Representatives: 50 distinct sales representatives are assigned to accounts.
Top Sales Representative: ID 321970 has the highest number of accounts.
Orders: 6,912 orders recorded.
Amount Spent: Maximum amount spent is $232,207; average amount spent is $3,343.
Sales Peaks: Highest sales recorded on December 31, 2016; highest order on December 1, 2016.
Customer Insights: Top customer ID 3411 made the highest order; top five customers are 4211, 4151, 1301, 1871, 4111.
Regional Performance: Northeast has the highest number of accounts and revenue; Region 1 has the highest count of sales representatives.
Web Events: Total of 9,073 web events; Direct channel has the highest number of web events; December 21, 2016, has the highest number of web events.
Top Channels: Direct, Facebook, Organic, Adwords, Banner.

Recommendations

Focus on Top-Performing Sales Representatives: Implement training and mentorship based on the performance of top sales reps.
Enhance Customer Retention: Develop personalized strategies for high-value customers to increase loyalty.
Optimize Regional Sales Strategies: Allocate resources and tailor strategies for top-performing regions.
Improve Web Event Channel Performance: Invest in optimizing high-performing channels and explore strategies for underperforming ones.
Leverage Seasonal Trends: Plan marketing and sales campaigns around peak sales periods to maximize revenue.

How to Use

Database Connection: Ensure you have access to the PostgreSQL database with the required tables.
Run Queries: Use the provided SQL queries to extract and analyze the data.
Interpret Results: Review the generated insights and charts to understand performance and trends.
Implement Recommendations: Use the recommendations to drive strategic decisions and improvements.

Tools and Technologies

PostgreSQL: Database management system
SQL: Query language used for data analysis
PowerPoint: Presentation software for reporting insights

