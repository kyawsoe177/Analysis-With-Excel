# Analysis of Sales Data from a Coffee Shop

<p align="justify"> This dataset captures transactional data from a coffee shop, detailing individual sales across various store locations. Each row represents a unique transaction and includes key information such as the 'transaction_id', 'transaction_date', 'transaction_time', 'transaction_qty', 'store_location', 'product_type', 'unit_price' and so on. </p>

<img src="https://github.com/user-attachments/assets/1d7ba1b8-4434-4337-a0dd-1749087f5c11" alt="Coffee shop dataset" width="900" height="200">
  
<p align="justify"> For in-depth analysis, we will first create a calculated filed, 'revenue', by multipying 'transaction_qty' and 'unit_price'. Then, time-based breakdowns including month, weekday, and hour are also extracted from time information. In the following sections, we will derive insights using pivot tables and charts. </p>

<img src="https://github.com/user-attachments/assets/e800eb38-6da0-44d4-835f-ef8be3977f5a" alt="New fields" width="200" height="100">

## Monthly Revenue Breakdown
<p align="justify">This chart presents the distribution of revenue over each month, offering insights into fluctuations in customer spending.</p>

<img src="https://github.com/user-attachments/assets/38ffd646-0e10-4d99-a9be-9c7de3c95612" alt="First chart" width="600" height="250">

## Daily Revenue Breakdown
<p align="justify">A detailed view of revenue generated along with total number of sales on a day-to-day basis.It is observed that there is no significant difference on sales among each day</p>

<img src="https://github.com/user-attachments/assets/aab8f5c1-8213-4dcb-be29-6482a66f17ad" alt="Second chart" width="600" height="250">

## Top Food Categories
<p align="justify">Highlights the best-performing food categories based on revenue. Coffee and tea dominate most volume of sales, occupying around 65% of total sales. By identifying the top-selling categories, we gain insights into customer preferences and product popularity.</p>

<img src="https://github.com/user-attachments/assets/6855d78b-be31-4b4d-8639-eb9b9f981022" alt="Third chart" width="600" height="250">

## Sales Pattern by Hour
<p align="justify">This examines how sales vary across different times of the day, revealing peak shopping hours and periods of low activity. Understanding these patterns helps in optimizing staffing, improving inventory availability, and scheduling promotions during high-traffic hours to maximize revenue. </p>

<img src="https://github.com/user-attachments/assets/a93084a4-36a7-4c11-b91b-dd59d90edc2d" alt="Fourth chart" width="600" height="250">

## Sales Performance Dashboard
This dashboard merges all previous charts and includes a list of top-selling food items from the coffee shop. It also features a slicer for filtering data by store location.

<img src="https://github.com/user-attachments/assets/17133a6f-6d6c-4b2c-ad11-86aa0c3137eb" alt="Dashboard" width="700" height="350">




