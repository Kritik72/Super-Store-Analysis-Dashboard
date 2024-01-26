## Super Store Sales Analysis: Dashboard 

## Problem Statement

My goal is to significantly contribute to the success of a business through the application of advanced data analysis techniques, with a particular emphasis on time series analysis. The primary focus is on providing valuable insights and precise sales forecasting.


### Steps followed 
- Step 1 : Load data into Power BI Desktop, dataset is a csv file.
- Step 2 : Starts Transforming the data as needed.
- Step 3 : Removed the Null Columns, Filtered Duplicates and Checked for the Data Types.
- step 4: Loaded the Transformed data into the powerBI Data View.

Snap of new calculated column: 

![image](https://github.com/Kritik72/Super-Store-Analysis-Dashboard/assets/58078426/77c1164e-adf2-469d-802b-064099f8cb6b)

Following DAX expression was created to find average delivery time.

        Avg_Delivery_Time = DATEDIFF(SuperStore_Sales_Dataset[Order Date],SuperStore_Sales_Dataset[Ship Date],DAY)


 # Report Snapshot (Power BI DESKTOP) Page-1
 
![Dashboard image-1](https://github.com/Kritik72/Super-Store-Analysis-Dashboard/assets/58078426/ad76881b-b4f1-42fa-9dfa-c50d3239ca50)

 # Report Snapshot (Power BI DESKTOP) Page-2
 
![Dashboard image-2](https://github.com/Kritik72/Super-Store-Analysis-Dashboard/assets/58078426/54302ad6-fe41-4a18-bf9d-0cff3bab3a18)
# Insights

One Sales Analysis Page and one Sales forecasting page was created on the powerbi Desktop.

Following inferences can be drawn from the dashboard;

### [1]  Remarkable total of 1.57 million in sales and 175.3k in profit over the span of two years across all four regions.

   Central Region Sales - 341.01k and Profit - 27.5k

   South Region Sales - 252.1k and Profit - 26.6k

   West Region Sales - 522.4k and Profit - 67.9k

   East Region Sales - 450.23k and Profit - 53.4k

           thus, We can conclude the highest sales and profit are from the WEST regions.
           
### [2] Top 3 Sales by Category.

    a) Offfice supplies - 643.7k
    b) Technology - 470.5k 
    c) Furniture - 451.5k   
  
  ### [3] Average Delivery Time
        As You can See from the visuals the average delivery time is 4 days.
### [4] Sales by State in the Sales forecasting page.
        Texas state comes to the highest total sales with 116k from all the states.

### [5] Monthly Insights for 2019 & 2020
- Identified August as the month with the lowest profit. (2019)
- Recognized December as the month with the highest profit. (2019)
- Revealed April as the month with the lowest profit.(2020)
- Highlighted December as the month with the highest profit.(2020)

## Implimented the Sales forecasting for 10 days: 
You can see from the visuals the sum of sales by Order Date from 1 january to 10 january.

- Made a new table from the super store sales data.

Below is the DAX query for SummarizeTable for Forecasting the data.

        SummarizeTable = SUMMARIZE(SuperStore_Sales_Dataset,SuperStore_Sales_Dataset[Order Date],SuperStore_Sales_Dataset[Sales])

The SummarizeTable contains two columns i.e Order date and Sales.

Snap of new SummarizeTable: 

![image](https://github.com/Kritik72/Super-Store-Analysis-Dashboard/assets/58078426/507e9312-dbc9-4893-b1b2-bd81bbbe1cde)

## Conclusion: 
Successfully employed advanced Data Analysis techniques, specializing in time series analysis, to unveil valuable insights, facilitate accurate sales forecasting, and create an interactive dashboard. The application of these methodologies has been instrumental in driving business success.
