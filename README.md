#  E-Commerce Sales Analysis Dashboard:

### Description:

This project aims to analyze sales data based on various product categories using Microsoft Excel. The dataset used for analysis is contained in the file E-Commerce Dashboard dataset.xlsx.
The dataset includes information such as Order ID, Order Date, Ship Date, Product Category, Sales, Profit, and more.

### Project Tasks:

1.	Sales and Profit Analysis: Prepare a table displaying sales and profit month-wise.
2.	Regional Sales Analysis: Create a table to visualize sales data region-wise.
3.	User Control Combo Box: Implement a user control combo box for selecting product categories.
4.	Column Chart Creation: Generate column charts for both the month-wise and region-wise tables.
5.	Dashboard Creation: Integrate all components into a comprehensive sales dashboard.

### Tools Required:
•	Microsoft Excel
•	Data Analysis Add-in

### How to Use:
1.	Open the E-Commerce Dashboard dataset.xlsx file in Microsoft Excel.
2.	Follow the instructions provided in the project tasks to perform the necessary analysis.
3.	Utilize the user control combo box to select specific product categories for detailed analysis.
4.	Refer to the column charts and dashboard for visual representations of the sales data.


## Formulas Used in the Project
### Formula 1: Sales and Profit Analysis

```excel
=SUMIFS('Sales Data'!$H:$H,'Sales Data'!$T:$T,Working!$F4,'Sales Data'!$F:$F,$S$3)
```
#### Description: 
This formula calculates the total sales amount ('Sales Data'!$H:$H) based on specified criteria. It sums the sales amounts where the product category matches the category selected in the 'Working' sheet ('Sales Data'!$T:$T,Working!$F4) and the month matches the month selected in cell $S$3

### Formula 2: Count of Orders Placed within 1 Day And Orders Placed Between 2 and 5 Days

```excel
=COUNTIFS('Sales Data'!$D:$D, "<=1")
```
#### Description: 
This formula counts the number of orders placed within a single day. It counts the occurrences where the difference between the Order Date and Ship Date ('Sales Data'!$D:$D) is less than or equal to 1 day.

```excel
=COUNTIFS('Sales Data'!$D:$D, ">=2",'Sales Data'!$D:$D, "<=5")
```
#### Description: 
 This formula counts the number of orders placed between 2 and 5 days. It counts the occurrences where the difference between the Order Date and Ship Date ('Sales Data'!$D:$D) is between 2 and 5 days.


## Expected Deliverables
The project is expected to deliver a comprehensive sales dashboard designed in Microsoft Excel. The dashboard should provide detailed analysis and insights into sales trends based on various product categories. Key deliverables include: 
#### 1)Sales and Profit Analysis: 
A table displaying sales and profit month-wise for easy visualization of trends over time.
#### 2)Regional Sales Analysis:
Visual representation of sales data region-wise to identify geographical trends and patterns.
#### 3)User Control Integration: 
Implementation of a user control combo box allowing users to select specific product categories for detailed analysis.
#### 4)Column Charts:
Creation of column charts depicting sales data, both month-wise and region-wise, for clear and intuitive visualization.
#### 5)Dashboard Creation:
Integration of all components into a cohesive and user-friendly sales dashboard providing actionable insights for stakeholders.
