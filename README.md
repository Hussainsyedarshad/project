Business Insights 360
---------------------------------------------------------------------------
Project Overview
AtliQ Hardware is growing rapidly in the recent years, and they have decided to implement the data analytics using PowerBi in their company for the first time to surpass their competitors in the market and to make data driven decisions. This project is hoped to give answers to the questions of stakeholder in terms all the aspects like finance, sales, marketing and supply chain.
--------------------------------------------------------------------

- Tech stacks
* SQL
* PowerBi Desktop
* Excel
* DAX language
* DAX studio (for optimizing the report)
* Project charter file
---------------------------------------------------------------
- PowerBI techniques Learnt
* What are all the questions should be asked before staring the project
* Creating calculated columns
* creating measure using DAX language
* Data modeling
* Using Bookmarks to switch between two visuals
* Page navigation with buttons
* Using divide function to prevent zero division errors
* creating date table using m language
* Dynamic titles based on the applied filters
* Using KPI indicators
* Conditional formatting the values in visuals using icons or background color
* Data validation techniques
* PowerBi services
* Publishing reports to PowerBi services
* Setting up personal gateway to set up the auto refresh of data
* PowerBi App creation
* Collaboration, workspace, access permissions in PowerBi services
 And more 
----------------------------------------------------------------------------
- GitHub
Uploading Large size files using GitHub LFS
Tracking the particular type of file extensions for LFS
-----------------------------------------------------------
- Business related terms
* Gross price
* Pre-invoice deductions
* Post-Invoice deductions
* Net Invoice sale
* Gross Margin
* Net sales
* Net profit
* COGC - cost of goods sold
* YTD - Year to Date
* YTG - Year to Go
* Direct
* Retailer
* Distributors
* Consumer
-------------------------------------------------------------------------------
- Company’s back ground
- 
AltiQ hardware is a company which has grown vastly in the recent years, and opened business all over the globe. It is a company which sells, computer and computer accessories through three mediums/channel
------------------------------------------------------------
Retailers
* Direct
* Distributors
Recently the company has faced a unforeseen loss by opening store in America based on the surveys, intuition and some excel analysis and also the company’s competitors has handful of analytics team to perform analysis and make data driven decision. So, the AltiQ hardware has no other option other than building their analytics team for data driven insights and decisions in the future to survive better in the industry.

Project kick off session, where you should get clear of for what and why this project and all other questions you have with regards to the project

- Questions to ask before starting with dashboard
--------------------------------------------------------------------------------
* What is the objective of building this PowerBi dashboard?

* In what terms the success of this project will be measured?

* What will be time dead-line of the project?

* do the stakeholders expecting pre-view before the actual release?

* What are all the hopes stakeholders have out of this project?

* what are all fears the stakeholder have in terms of building this dashboard?

* Who are all will be using this dashboard and for what purpose?

* what are all expectation the stakeholders have, by the completion of this project?

* What can go wrong while building this project?

* what are all the resources/ data needed to build this dashboard?

* is there any inputs from stakeholders in terms of design and views of the dashboard?

After the project kick off meetings, the data engineering team has given the data as per the request of data analytics team, let’s explore them.
-------------------------------------------------------------------------
- Dataset Understanding.

Understanding what data is available will be more helpful while doing analysis. before jumping on to the analysis get good understanding of what are data available.

Dimension table : It will have the static data like details of customer and products

Fact table : It will have the data about the transactions
-------------------------------------------------------------------------
gdb041:
 - dim_customer

   27 distinct markets (ex India, USA, spain)

   .75 distinct customers thorough out the market

    .2 types of platforms

     .Brick & Motors - Physical/offline store

     .E-commerce - Online Store (Amazon, flipkart)

    *Three channels

     .Retailer

     .Direct

     .Distributors

- dim_market

  .27 distinct markets (ex India, USA, spain)

  .7 sub-zones

  .4 regions

  .APAC

  .EU

  .nan

  .LATAM

- dim_product

  .Divisions

  .P & A

  .Peripherals

  .Accessories

  .PC

  .Notebook

  .Desktop

  .N & S

  .Networking

  .Storage

  .There are 14 different categories, Like Internal HDD, keyboard

  .There are different variants available for the same product
  
- fact_forecast_monthly

  .This table is used to forecast the customer’s need in advance, which can help in


  .Higher customer satisfaction

  .Reduced cost in warehouses for storage purpose

  .The table is denormalized by data engineering team, as it is a data warehouse which is aimed to be used for analytical work.

  .All the date of the month will be replaced by the start date of the month

  .It will have all the column names and in the end it will have the forecast quantity need of the customer
  
- fact_sales_monthly

  .This table is more or less is same as fact_forecase_monthly table, but the last column has the value of sold quantity instead of forecast value.
-----------------------------------------------------------------------------------------
gdb056

- freight_cost

This table has details of travel cost and other cost for each market with fiscal year
- gross_price

  Has the details of gross prices with product code
- manufacturing_cost

  Has the details of manufacturing cost with product code with year
- Pre_invoice_dedutions

  Has the details of pre invoice deductions percentage for each cutomer with year
- Post_invoice_deductions

  Post invoice deductions and other deductions details
- Importing data into PowerBi

As the database is MySQL in this project, we need to import the datasets from Mysql database to PowerBi by providing the Database access credential

----------------------------------------------------------------------------------
- Data Model
* Data modeling plays a vital role and is considered as the basement of report. All the visuals will be build upon the data model.
* Poor data modeling affects the over all performance of the report.
* Following Good practices of data modeling is must. Refer this page to get to know the good practices Blog
* In this project, we have followed Snowfall data modeling method.
----------------------------------------------------------------------------------

Dashboard designing
Based on the mock ups received as requirement, the team will start designing the visuals and create measure as and when required

Home view
<img width="1457" height="818" alt="Screenshot 2025-12-03 122407" src="https://github.com/user-attachments/assets/1a76b1c9-d3ee-4763-93af-f3c5f2ebf93b" />
---------------------------------------------------------------------------------------------------

Info

Sales View

Marketing View

Supply chain View

Executive View

------------------------------------------------------------------------
Overall Report
<img width="1479" height="796" alt="Screenshot 2025-12-03 122551" src="https://github.com/user-attachments/assets/72e53a19-a5f0-4e35-bd2f-c3e5c3c33ea2" />
------------------------------------------------------------------------------

Info Page
<img width="1499" height="813" alt="Screenshot 2025-12-03 122610" src="https://github.com/user-attachments/assets/cf53c8e9-268b-488f-a5d4-8ddb9c927474" />
----------------------------------------------------------------------------------------------------
Finance View
<img width="1462" height="809" alt="Screenshot 2025-12-03 122428" src="https://github.com/user-attachments/assets/7d2302fe-e62f-4e32-91aa-4b027610c4d1" />
---------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------

Sales View
<img width="1448" height="808" alt="Screenshot 2025-12-03 122451" src="https://github.com/user-attachments/assets/828fffb0-fb63-42b2-96c1-3b67288fbc72" />
---------------------------------------------------------------------

Marketing View
<img width="1451" height="818" alt="Screenshot 2025-12-03 122529" src="https://github.com/user-attachments/assets/49329b3b-43bb-4857-beaa-49bdd856e6d1" />
----------------------------------------------------

Supply chain View
<img width="1479" height="796" alt="Screenshot 2025-12-03 122551" src="https://github.com/user-attachments/assets/1edf0660-f414-4a03-853b-858a26833fb4" />
--------------------------------------------------------------------------

Executive View
<img width="1499" height="813" alt="Screenshot 2025-12-03 122610" src="https://github.com/user-attachments/assets/d08bc8bb-746c-4e94-b5c8-e58669b9551a" />
-------------------------------------------------------------------------

Products
<img width="1450" height="815" alt="Screenshot 2025-12-03 122630" src="https://github.com/user-attachments/assets/c02b4fd0-67ba-4a75-9a08-51d1a8626a14" />
-----------------------------------------------------------------------------

you can find the full report file here : Report

Project Outcome
By using this report, decisions can be taken based on the data. Further it will help in answering n number of why questions based on the situations.
