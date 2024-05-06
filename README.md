<div align='center'> <h1> PIZZA SALES ANALYSIS </div>

#### Tools used: Excel, Power BI

 Dataset used: [Click to view](file:///C:/Users/hp/OneDrive/Pizza_Sales-Data-1.htm) 

 Power BI Dashboard: [Click to view](https://1drv.ms/i/c/94c0edc81177dbde/EanaV70hsGRFrCNjLdzoZMYBjg9NKUqg7RPGf0WeOd4prQ?e=eMcCvl)
 
 Power BI Dashboard: [Click to interact](https://app.powerbi.com/view?r=eyJrIjoiYTNiNjE0NzUtNDYzNC00NzQ5LWE4MzgtODIwM2NlZWEyNTVlIiwidCI6IjI3MGRhZWVlLTdkMWYtNDQwZC1hMDYxLTQzOWMzMGFhYjUwMSJ9)

## About this project

This project aims to analyze sales data spanning pizza types across various company locations over a three-year period.

![image](https://github.com/Weefred/Pizza_Sales_Analysis/blob/main/pizza%20sales%20dashboard.png)

## APPLIED STEPS

#### The ETL Process

1. **Extract**: The dataset for this project was sourced from an Excel workbook, and imported into the Power Query Editor for transformation. It consists of 1,000,001 rows and 8 columns.

2. **Transform**: Two new columns were created to determine the sales before discount and actual sales figures. They include:

             Sales before discount: using the formular:  = ([Unit Price] *[Quantity])
             Sales: using the formular: = ([Unit Price] *[Quantity]) *(1- [Sales Discount])) 
             
In addition, two extra columns were created using the time and date columns to analyze sales patterns based on both the time of day and day of the week. They include:

                 Period of day =IF(HOUR(PIZZA[Time])<12,"Morning",IF(HOUR(PIZZA[Time])<16,"Afternoon","Evening"))
                 Day of week = FORMAT(PIZZA[Date],"dddd")
                 
3. **Load**: Data was then loaded into Power BI for visualization.

4. **Exploratory Data Analysis**: EDA involved exploring the sales data to answer the following key questions.

- Which year records the peak in sales figures and how do they compare to other years?

- Which pizza types demonstrate the highest sales performance?

- How does overall pizza sales performance vary across the different locations?

- At what period of day do we have the highest sales?

- What is the impact of sales discounts on overall revenue and profitability?

## Insights

1. Among the three years, 2018 emerges as the peak sales year recording ₦5.78bn in revenue, closely followed by 2019 with ₦5.77bn. However, year 2020 saw a significant decline to ₦1.54bn.

2. Margarita is the top-selling pizza with ₦2.1M in revenue and a total of 728,618 quantity sold, followed closely by Beef Suya and Meatzaa. Conversely, BBQ Philly Steak and Extravaganza exhibit lower sales. Possible reasons could be differences in customer preferences or marketing effectiveness.

3. Variations in pizza sales performance across different locations are evident, with Ikeja leading at ₦4.91bn. Strong performances are also observed in Ikoyi. In contrast, Surulere recorded the lowest sales.

4. Peak sales, totaling ₦5.2bn in revenue, are observed during the day, potentially driven by factors such as increased consumer activity, workday schedules, and promotional strategies. While evening sales amount to ₦2.6bn.

5. The comparison between sales before and after discounts shows a slight decrease in revenue from ₦13.6bn to ₦13.1bn indicating minimal impact of discounts on overall sales.

## Recommendations

**Review Product Offerings**: Consider introducing new flavors, toppings, or menu items to attract a wider customer base and cater to changing tastes.

**Feedback Collection**: Implement mechanisms for collecting feedback from customers in each location to understand their preferences, satisfaction levels, and areas for improvement.

**Regional Strategy**: With Ikeja and Ikoyi as our leading customer base, consider expanding operations by opening new outlets and increasing marketing efforts. For other locations, more effort should be put into advertising to create greater awareness.

**Maximize Peak Sales Periods**: Capitalize on peak sales periods during the day by allocating resources and promotional efforts. To boost evening sales, consider offering online ordering and delivery services. Also create a cozy dining atmosphere.

**Strategic Timing**: Offer discounts during off-peak hours or slower sales periods as an incentive for customers to visit during these times and increase foot traffic and sales.

