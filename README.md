# 🍽️ Zomato Analytics Dashboard - Power BI

## 📖 Introduction
The **Zomato Analytics Dashboard** is a data visualization project built using Power BI to provide deep insights into food delivery performance, restaurant reviews, and customer preferences. This dashboard helps stakeholders identify key trends, optimize delivery operations, and enhance customer satisfaction.

---

## 🎯 Objectives
- Track order and delivery performance.
- Monitor restaurant reviews and average customer ratings.
- Analyze customer behavior and preferences.
- Visualize data for real-time decision-making.
- Improve operational efficiency using key performance indicators (KPIs).

---

## 📊 Key Performance Indicators (KPIs)
| KPI Name                  | Description                                                            |
|---------------------------|------------------------------------------------------------------------|
| **Total Orders**          | Total count of orders within a selected date range.                    |
| **Average Delivery Time** | Average time (in minutes) taken for deliveries.                        |
| **Average Order Value**   | Total revenue divided by the total number of orders.                   |
| **Customer Satisfaction** | Average rating given by customers (scale of 1 to 5).                   |
| **Discount Utilization**  | Percentage of orders where a discount was applied.                     |

---

## 📈 Visualizations
| Chart Name                | Description                                                              |
|---------------------------|--------------------------------------------------------------------------|
| **Total Orders Trend**    | Line chart showing order volume over time (daily, weekly, monthly).      |
| **Delivery Time Analysis**| Bar chart showing average delivery time by city.                         |
| **Top Restaurants**       | Horizontal bar chart showing top 10 restaurants by revenue.              |
| **Ratings Distribution**  | Pie or bar chart showing breakdown of customer ratings (1 to 5 stars).   |
| **Cuisine Popularity**    | Bar chart displaying the most popular cuisines based on order volume.    |

---

## 🧮 Filters
The dashboard supports dynamic filtering to enhance user interactivity:

- **Date Range**: Filter data for specific time periods.
- **City/Location**: Filter based on customer or restaurant locations.
- **Cuisine Type**: View data by selected cuisines (e.g., Indian, Chinese, Italian).
- **Rating Range**: Filter based on average rating (e.g., 3 stars and above).
- **Discount Applied**: Toggle to view discounted or non-discounted orders only.

---

## 📂 Data Sources
The dashboard uses the following datasets:

### 1. Orders Dataset
- `Order_ID`
- `Customer_Name`
- `Customer_Location`
- `Restaurant_Name`
- `Cuisine`
- `Order_Date`
- `Delivery_Time_Minutes`
- `Order_Amount`
- `Is_Discount_Applied`

### 2. Restaurant Dataset
- `Restaurant_Name`
- `Restaurant_Location`
- `Cuisine`
- `Rating`
- `Total_Reviews`

### 3. Reviews Dataset
- `Review_Text`
- `Rating`
- `Review_Date`
- `Customer_Name`

---

## 🔧 Functional Requirements

| **View Name**               | **Description**                                             | **Required Columns**                                       |
|----------------------------|-------------------------------------------------------------|------------------------------------------------------------|
| Total Orders KPI           | Displays total orders placed within the selected period.    | Order_ID                                                   |
| Average Delivery Time KPI  | Shows the average delivery time for orders.                 | Delivery_Time_Minutes, Order_ID                            |
| Average Order Value KPI    | Calculates the average value of all orders.                 | Order_Amount, Order_ID                                     |
| Customer Satisfaction KPI  | Displays the average rating given by customers.             | Rating, Review_Date                                        |
| Discount Utilization KPI   | Shows the % of orders with discounts applied.               | Is_Discount_Applied, Order_ID                              |
| Total Orders Trend Chart   | Line chart showing order trends over time.                  | Order_Date, Order_ID, Customer_Location                    |
| Delivery Time Chart        | Bar chart analyzing delivery time by city.                  | Delivery_Time_Minutes, Customer_Location                   |
| Top Restaurants Chart      | Bar chart showing the top 10 restaurants by revenue.        | Restaurant_Name, Order_Amount, Restaurant_Location         |
| Ratings Distribution Chart | Pie chart showing distribution of customer ratings.         | Rating, Order_ID                                           |
| Cuisine Popularity Chart   | Bar chart highlighting the most popular cuisines.           | Cuisine, Order_ID                                          |

---

## 🛠️ Tools Used
- **Power BI Desktop** for building dashboards
- **Excel/CSV** files as data sources
- **DAX** for calculated columns and measures
- **Power Query Editor** for data cleaning and transformation

---

## 📌 Conclusion
This Zomato Analytics Dashboard enables data-driven decision-making for food delivery operations and customer engagement strategies. By leveraging key KPIs and visual insights, businesses can improve customer satisfaction, optimize delivery times, and identify high-performing restaurants.

