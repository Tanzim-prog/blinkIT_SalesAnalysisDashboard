# blinkIT Sales Analysis Dashboard

#### Dashboard Link: https://drive.google.com/file/d/1L2PtTbgz7C3b9G9Jm5ol7eopZi7CXH0k/view?usp=drive_link

## Overview

This dashboard will help the organization to understand their sales better from different perspecttives. It will help the organizaions to know about their total sales, average sales, number of items sold. This dashboard will also help them to know about the average of rating people gave them.

### Requirements

#### KPI Requirements
- Total Sales
- Average Sales
- Number of items sold
- Average Rating

#### Other Requirements
- Total sales by fat content
- Total sales by item type
- Fat contentt by outlet for otal sales
- Total sales by outlet establishment
- Sales by outlet size
- Sales by outlet location
- All metrics calculationn by outlet type

### Steps followed

- Step 1: Requiremnets gathering
- Step 2: Data Walkthrough/ Data QC. During the QC two problems were found. One is two differentt entries had the same meaning so it was fixed usig 'Replace Values' option in Power Query. Another problem was there was several missing values in a attribute. But as the attribute was not in use it wasn't really a problem for this project.
- Step 3: Some new measures, Total Sales, Average Sales, Number of items, Average Rating, were introduced as per The KPI requirements. Data Analysis Expressions (DAX) query was used to calculate these measures.

#### DAX Calculation    
Total Sales = SUM('BlinkIT Grocery Data'[Sales])

Avg Sales = AVERAGE('BlinkIT Grocery Data'[Sales])

No of Items = COUNTROWS('BlinkIT Grocery Data')

Avg Rating = AVERAGE('BlinkIT Grocery Data'[Rating])

![KPI](https://github.com/user-attachments/assets/9da28573-adc8-4896-9e2e-8f156b2d38c5)

- Step 4: Created a new metrics table using data modeling technique in power bi which includes the kpi requirements
- Step 5: Created a donut chart based on fat content
- Step 6: Created a clustered bar chart to present Fat Content by Outlet Location
- Step 7: Created a stacked column chart to present item types
- Step 8: Created a line chart to visualize Total Sales against Outlet Establishment Year
- Step 9: Created a donut chart to visualize Total Sales based on Outlet Size
- Step 10: Created a funnel chart based on Total Sales and Outlet Location Type
- Step 11: Generated a matrix chart based on Outlet Types. Through that matrix 5 different parameters were visualized including Total Sales, Average Sales, Number of Items, Item Visibility and Average Rating. Here Item Visibilitty was presented as item count. All those attributes were presented on the right side of every Outlet Type.
![Outlet Type Step 11](https://github.com/user-attachments/assets/51754376-a9d3-48a6-bd89-0d9f3ef90a2d)

- Step 12: Created a filter panel to easily filter out using params like outlet location type, size and item type
![Filter Panel Step 12](https://github.com/user-attachments/assets/2f4b684a-8853-401d-9b85-5c15bc631baa)

### Insights
A single page report was generated in Power BI Desktop
![Dashboard](https://github.com/user-attachments/assets/9d37d531-bd4b-4c2c-9097-b5c35e8f4985)

#### [1] Total Sales in cash: 1.2 Million Dollar
#### [2] Average Sales in cash: 141 Dollar
#### [3] Number of items sold: 8523
#### [4] Average rating from the critics: 3.9
