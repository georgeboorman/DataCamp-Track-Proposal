# **Create a Sample Exercise**

This exercise is from Chapter 1 Basics of Commercial Data, Lesson 1.2 Sales Performance, within the **Analyzing Commercial Metrics Course**. 

## Exercise Title: Calculating Customer Lifetime Value, Part 1

Customer Lifetime Value (CLV) is a crucial metric for any company in understanding the total amount of revenue they can reasonably expect from a single customer. 
To calculate CLV, the following steps are required:
1.	Average Order Size = Total Revenue / Total Number of Orders
2.	Average Order Frequency = Total Number of Orders / Total Number of Customers
3.	Average Customer Value = Average Order Size / Average Order Frequency
4.	Average Customer Lifespan = First Order Date – Last Order Date
5.	Customer Lifetime Value = Average Customer Lifespan / Average Customer Value

In this this exercise you will complete the first three steps to obtain Average Customer Value, then in the next exercise you will find the Average Customer Lifespan and use to determine Customer Lifetime Value.

`pandas` has been imported as `pd`, and a DataFrame named `customer_data` is already loaded for you containing data on customers and sales for an e-commerce company.  

### **Instructions** <br>
•	Create a column in `customer_data` called `average_order_size`, which contains the sum of dividing `total_revenue` by `total_orders`. 

•	Calculate `average_order_frequency` and store as a new column in `customer_data` using the formula provided in the description. 

•	Add `average_customer_value` as a column in `customer_data`, dividing `average_order_size` by `average_order_frequency`.

•	Print descriptive statistics for the newly created columns.

### **Code to be Completed**

#### Calculate average order size
customer_data[‘average_order_size‘] = customer_data[‘total_revenue’] / customer_data[‘\_\_\_\_’]

#### Calculate average order frequency
customer_data[‘\_\_\_\_’] = customer_data[‘\_\_\_\_’] / customer_data.shape [‘\_\_\_\_’]

#### Calculate average customer value
customer_data[‘\_\_\_\_’] = customer_data[‘average_order_size’] / customer_data[‘\_\_\_\_’]

#### Print the descriptive statistics for the three newly created columns
customer_data[[‘average_order_size’, ‘\_\_\_\_’, ‘\_\_\_\_’]].’\_\_\_\_’()

### **Answers**

#### Calculate average order size
customer_data[‘average_order_size‘] = customer_data[‘total_revenue’] / customer_data[‘total_orders’]

#### Calculate average order frequency
customer_data[‘average_order_frequency’] = customer_data[‘total_orders’] / customer_data.shape [0]

#### Calculate average customer value
customer_data[‘average_customer_value’] = customer_data[‘average_order_size’] / customer_data[‘average_order_frequency’]

#### Print the descriptive statistics for the three newly created columns
customer_data[[‘average_order_size’, ‘average_order_frequency’, ‘average_customer_value’]].describe()
