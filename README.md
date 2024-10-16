# Customer Analytics Tableau Dashboards

## Overview
This project analyzes customer shopping behavior using **Tableau** to create interactive dashboards based on a customer shopping dataset. The dataset contains over **5,000 transactions** with information on customer demographics, product categories, and shopping malls. The project delivers insights on **sales trends**, **customer segmentation**, and **spending patterns** that can inform **targeted marketing strategies**.

### Dashboards Created:
1. **Overall Sales Performance Dashboard**
2. **Customer Segmentation Dashboard**

## Dashboard Preview

![Dashboard Consumer Analytics](./Dashboard%20images/Dashboard%20Consumer%20Analytics.PNG)

## Data
The dataset contains the following fields:
- **Invoice Number**: Unique identifier for each transaction
- **Customer ID**: Unique identifier for each customer
- **Gender**: Gender of the customer (Male, Female)
- **Age**: Age of the customer
- **Category**: Product category (Clothing, Shoes, Technology, etc.)
- **Quantity**: Number of items purchased
- **Price**: Price per item
- **Total Sales**: Price * Quantity (calculated)
- **Payment Method**: Cash, Credit Card, or Debit Card
- **Invoice Date**: Date of the purchase
- **Shopping Mall**: Mall where the transaction took place

### Preprocessing
The dataset was preprocessed using **Python (Pandas)** to:
- **Handle missing values**
- **Convert invoice dates** to a proper datetime format
- **Create new features**, such as:
  - **Total Sales**: (Price * Quantity)
  - **Age Groups**: Created age bins (e.g., 11-20, 21-30, etc.) for better segmentation
  - **Invoice Year/Month**: Extracted from invoice date for trend analysis

## Tableau Dashboards

### 1. **Overall Sales Performance Dashboard**
This dashboard provides a high-level overview of sales performance across different dimensions:
- **Sales Trends**: A time series chart that visualizes total sales over the years 2021, 2022, and 2023.
- **Sales by Category**: Bar chart showing sales by product categories such as Clothing, Shoes, Technology, etc.
- **Payment Methods**: Visualized payment types across different malls and total sales by cash, credit card, and debit card.
- **KPI Summary**: Includes key metrics such as:
  - **Total Sales**: $251,505,794
  - **Number of Transactions**: 99,457
  - **Average Order Value**: $2,529
  - **Average Quantity per Transaction**: 3.003

#### Insights:
- The **Clothing** category generated the highest sales across all years.
- **Credit Card** payments accounted for the majority of transactions, showing a customer preference for cashless payments.
- **Kanyon** and **Mall of Istanbul** are the highest-grossing malls.

### 2. **Customer Segmentation Dashboard**
This dashboard segments customers based on **age**, **gender**, and **shopping behavior**:
- **Sales by Age Group**: Bar chart showing the sales contribution by different age groups. The **31-40 age group** contributed the highest sales, totaling **$189,977 more** than other groups.
- **Sales by Gender**: A pie chart that breaks down total sales by gender, showing that **women consistently outspend men across all categories**, with a total difference of **$48,908,478**.
- **Sales by Category (Gender)**: A stacked bar chart visualizing spending habits by gender across categories such as Clothing, Shoes, and Technology. Women spent **$22,506,601** more on Clothing than men.
- **Sales by Mall**: A bar chart comparing total sales across shopping malls. **Mall of Istanbul** ranked first, with **$50,687,482** in total sales, closely followed by **Kanyon** at **$50,554,231**.

#### Insights:
- **Women** outspent men across all product categories, making them a key demographic for high-value sales, particularly in **Clothing**.
- **Mall of Istanbul** and **Kanyon Mall** were the most popular malls, with a small difference in total sales.
- **Age group 31-40** is the highest-spending demographic, offering significant opportunities for targeted marketing campaigns.

## Tools Used
- **Tableau**: Used to create interactive dashboards for data visualization.
- **Python (Pandas)**: Used for data preprocessing, feature engineering, and initial exploration.
  
## Key Features
- **Interactive Visualizations**: Users can filter by categories, gender, and age to dynamically explore data trends.
- **KPI Tracking**: Displays key metrics like total sales, average order value, and customer demographics.
- **Actionable Insights**: Provides insights into which age group and gender are driving the most sales, helping businesses with segmentation and marketing strategies.

## How to Use
1. **Download** the Tableau Packaged Workbook (`.twbx`) from the repository.
2. Open the `.twbx` file in **Tableau Desktop** or **Tableau Public**.
3. Explore the **Overall Sales Performance** and **Customer Segmentation Dashboards** by interacting with filters and charts to analyze the data.

## Conclusion
This project showcases how to use Tableau for data analysis and customer segmentation to derive actionable insights from raw data. By visualizing key metrics and customer behavior, businesses can make informed decisions about their marketing strategies, product focus, and customer targeting efforts.
