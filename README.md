# Analysis with Excel
<p align="justify"><b>Problem Statement :</b> The business lacked a centralized, visual, and easily interpretable way to monitor sales performance across different store locations, product categories, time periods, and customer behavior patterns. Decision-makers were relying on fragmented data, making it difficult to identify trends, optimize inventory, and plan targeted marketing or operational strategies
</p>

<p align="justify"><b>Goal :</b> The goal of this project is to demonstrate data cleaning in Excel and design and develop an interactive sales dashboard that enables business stakeholders to monitor and analyze performance across multiple dimensions, including store locations, product categories, time of day, and customer purchasing trends. 
</p>

<p align="justify"><b>Tools used :</b> Mircrosoft Excel</p>

<p align="justify"><b>Data :</b> Employee dataset for data cleaning and coffee shop sales dataset for data analysis</p>


## Cleaning Employee Dataset
This dataset contains basic employee information within an organization. It includes the following fields, 'Employee ID', 'Name', 'Date Hired', 'Department', 'Status'. 
The primary focus will be on cleaning this dataset.

### Creating a duplicate
To be safe, we will start by duplicating the dataset in case of any issues.

<img src="https://github.com/user-attachments/assets/d5227737-b976-42db-b2d0-f5717964ff6b" alt="Duplicate worksheet" width="250" height="100">


There are noticeable inconsistencies in the data, including variations in letter casing and the presence of null values.

<img src="https://github.com/user-attachments/assets/7927e839-88dd-41de-b306-4daf1065b969" alt="Messy data" width="400" height="200">


### Cleaning department column
There are missing entries in the 'Department' column. We will apply conditional formatting to highlight these and any other null values.

<img src="https://github.com/user-attachments/assets/eda08ac2-8e78-4ab1-a608-6ef69e6baeae" alt="Conditional formatting" width="100" height="100">

After that, those values will be replaced with 'Unassigned' using the following IF command.
````
=IF(OR(D2="", D2="none"), "Unassigned", D2)
````

### Cleaning duplicates
Identifying duplicate values is also an important step in data cleaning. We will look for duplicates in 'Employee ID' and 'Name' columns with conditional formatting again.

<img src="https://github.com/user-attachments/assets/9aefca06-6fef-46d5-98c3-11e989acd3cc" alt="Conditional formatting" width="200" height="100"><br/>

The duplicate values are highlighted in green.

<img src="https://github.com/user-attachments/assets/a7b9f2bf-7761-41f9-9c8e-ec6ef81b9d83" alt="Conditional formatting" width="100" height="150"><br/>

### Fixing inconsistensies 
Lastly, we'll address inconsistencies in letter casing such as 'AARON HERNANDEZ' and 'operations'  within the 'Name,' 'Department,' and 'Status' columns using '=PROPER()'.

<img src="https://github.com/user-attachments/assets/bc3cc525-529c-4ce6-a086-c604ee03c6d0" alt="Conditional formatting" width="300" height="150"><br/>

The dataset is now ready for further analysis.

## Analysis of Coffee Shop Data using Pivot Table

<p align="justify"> This dataset captures transactional data from a coffee shop, detailing individual sales across various store locations. Each row represents a unique transaction and includes key information such as the 'transaction_id', 'transaction_date', 'transaction_time', 'transaction_qty', 'store_location', 'product_type', 'unit_price' and so on. </p>

<img src="https://github.com/user-attachments/assets/1d7ba1b8-4434-4337-a0dd-1749087f5c11" alt="Coffee shop dataset" width="900" height="200">
  
<p align="justify"> For in-depth analysis, we will first create a calculated filed, 'revenue', by multipying 'transaction_qty' and 'unit_price'. Then, time-based breakdowns including month, weekday, and hour are also extracted from time information. In the following sections, we will derive insights using pivot tables and charts. </p>

<img src="https://github.com/user-attachments/assets/e800eb38-6da0-44d4-835f-ef8be3977f5a" alt="New fields" width="200" height="100">

## Pivot Tables

We are going to use a pivot table to analyze the data, allowing us to efficiently summarize, filter, and compare key metrics such as sales performance by category, and across different time periods.

<img src="https://github.com/user-attachments/assets/d84dbd25-ff42-429b-93d3-b334ddcbb346" alt="Pivot tables" width="180" height="250">

### Monthly revenue breakdown
<p align="justify">This chart presents the distribution of revenue over each month, offering insights into fluctuations in customer spending.</p>

<img src="https://github.com/user-attachments/assets/38ffd646-0e10-4d99-a9be-9c7de3c95612" alt="First chart" width="600" height="250">

### Daily revenue breakdown
<p align="justify">A detailed view of revenue generated along with total number of sales on a day-to-day basis.It is observed that there is no significant difference on sales among each day</p>

<img src="https://github.com/user-attachments/assets/aab8f5c1-8213-4dcb-be29-6482a66f17ad" alt="Second chart" width="600" height="250">

### Top food categories
<p align="justify">Highlights the best-performing food categories based on revenue. Coffee and tea dominate most volume of sales, occupying around 65% of total sales. By identifying the top-selling categories, we gain insights into customer preferences and product popularity.</p>

<img src="https://github.com/user-attachments/assets/6855d78b-be31-4b4d-8639-eb9b9f981022" alt="Third chart" width="600" height="250">

### Sales pattern by hour
<p align="justify">This examines how sales vary across different times of the day, revealing peak shopping hours and periods of low activity. Understanding these patterns helps in optimizing staffing, improving inventory availability, and scheduling promotions during high-traffic hours to maximize revenue. </p>

<img src="https://github.com/user-attachments/assets/a93084a4-36a7-4c11-b91b-dd59d90edc2d" alt="Fourth chart" width="600" height="250">

### Sales performance dashboard
This dashboard merges all previous charts and includes a list of top-selling food items from the coffee shop. It also features a slicer for filtering data by store location.

<img src="https://github.com/user-attachments/assets/17133a6f-6d6c-4b2c-ad11-86aa0c3137eb" alt="Dashboard" width="700" height="350">

## Key Insights

- Sales show the highest growth in May and June, with steady increases from February onward.
- Approximately 65% of total sales come from tea and coffee categories.
- Most purchases occur between 7 AM to 11 AM, with a peak around 10 AM.
- Sales are consistently higher Monday to Friday, with a dip on Saturday.

## Actionable Recommendations

- Launch seasonal promotions or loyalty campaigns ahead of peak months to encourage early purchases.
- Introduce bundled offers featuring the most popular categories (e.g., coffee and pastry) to drive upselling opportunities.
- Offer early bird discounts or “coffee happy hours” during off-peak hours to boost sales during slower periods.
- Launch weekend-exclusive menu items or events to encourage habitual weekday buyers to return on weekends.
- Use customer favorites in featured menus or loyalty rewards to increase engagement, drive repeat visits, and enhance customer satisfaction through personalized offerings.
