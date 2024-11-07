# LITA_Capstone_Project

# LITA-Capstone-Documentation

### Project Title: LITA Capstone Analysis

[Project Overview](#Project-Overview)

[Data Sources](#Data-Sources)

[Tools Used](#Tools-Used)

[Data Cleaning and Preparation](#Data-Cleaning-and-Preparation)

### Project Overview
---
This Data Analysis project aims to generate insights into the Sales Performance and Customer Data of the Capstone project over the past year. By analysing the various parameters in the data received we seek to gather enough insights to make reasonable decisions which then enable us to tell compelling stories around our data from the insights gotten and to know the best performance from our data.

### Data Sources
---
The primary sources of data used here is LITA Capstone Dataset. [Accessible here](https://github.com/user-attachments/files/17645847/LITA.Capstone.Dataset.xlsx)


### Tools Used
---
- Microsoft Excel 
    1. For Data Cleaning 
    2. For Analysis
    3. For Data Visualization
     
- SQL - Structured Query Language for Querying of Data
   1. For generating some outcomes using simple queries, just like are stated below.
   2. Also creating tables of simple outcomes like grouping either by Region or by Products.
      
- PowerBI
  For intense cleaning and wrangling of the Data.
  Also for visualizations.

### Data Cleaning and Preparations
---
In the initial phase of the Data Cleaning and preparations, we perform the following action;
1. Data loading and Inspection
2. Handling missing variables
3. Data Cleaning and formatting

   ### Exploratory Data Analysis
   ---
   EDA involves the exploring of the Data to answer some questions about the Data such as;
   - What is the overall sales trend
   - Which product are top sellers
   - What are the products on peak sales?
  
     ### Data Analysis
     ---
     This is where we include some basic lines of code or queries or even some of the DAX expressions used during your analysis;

     ```SQL
     SELECT * FROM Dbo.LITACapstone
     ````
    
````SQL
-----------find the highest-selling product by total sales value---------
select Top 1 Product, sum(Sales) as TotalSales 
from LITACapstone
Group by Product
````

````SQL
Select * from [dbo].[CustomerData]

----------retrieve the total number of customers from each region----------
Select Count(CustomerName) as Customers_per_Region, Region
from [dbo].[CustomerData]
Group by Region
````

````SQL
----------find the most popular subscription type by the number of customers--------
Select Top 1 SubscriptionType,Count(CustomerId)
from CustomerData
Group by SubscriptionType
````


### Data Visualization

![Screenshot (7)](https://github.com/user-attachments/assets/8dfbaf21-039d-4d59-bc66-5e947c2c2dc5)

![Screenshot (8)](https://github.com/user-attachments/assets/4bc0d880-7979-4a53-bf06-c462e35012b9)

![Screenshot (11)](https://github.com/user-attachments/assets/acec2ea1-8385-4c07-8acb-88fcdfbbd0dd)

![Screenshot (14)](https://github.com/user-attachments/assets/fdef5cef-5e92-4169-94fd-aa92a42b0d11)

![Screenshot (15)](https://github.com/user-attachments/assets/4d1ec88c-fc68-4542-a4ac-dd38b126e74f)

![Screenshot (16)](https://github.com/user-attachments/assets/2379502b-1baf-4039-93d5-6d442d005c8d)

![Screenshot (17)](https://github.com/user-attachments/assets/55acb2fa-5262-4c65-8114-c5b423f62c47)

![Screenshot (18)](https://github.com/user-attachments/assets/b929ba5f-5a13-4c05-99ce-38a2de2a25d2)

![Screenshot (19)](https://github.com/user-attachments/assets/efd4ffa6-f32f-4373-97b2-5e6ba3139168)

![Screenshot (20)](https://github.com/user-attachments/assets/8179b50d-f29a-4818-954d-1ca1dc5470ed)

![Screenshot (21)](https://github.com/user-attachments/assets/bf404301-3c80-454d-8238-e66e2aea4f05)

![Screenshot (22)](https://github.com/user-attachments/assets/b54e6572-b3ec-4461-b17f-1c03609ee006)

![Screenshot (24)](https://github.com/user-attachments/assets/b0bde723-0106-47fb-a7d5-4bc5dd40bcda)

![Screenshot (25)](https://github.com/user-attachments/assets/577221af-2fd8-435b-a5bc-19aa59e3aea9)




