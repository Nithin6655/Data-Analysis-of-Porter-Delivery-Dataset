# Porter Delivery Data Analysis
## Project Overview

This project analyzes Porter delivery data to understand factors affecting delivery time, order demand, and operational efficiency. The goal is to identify patterns in delivery delays and provide actionable insights to improve performance.

## Objectives
Analyze delivery time distribution and identify outliers
Understand demand patterns (peak hours and days)
Study impact of operational load on delivery time
Evaluate performance across markets and store categories
Identify key factors influencing delivery delays
Dataset Description

The dataset contains information about delivery orders including:

Order timestamps (created_at, actual_delivery_time)
Store details (store_id, store_primary_category)
Order details (total_items, subtotal)
Operational metrics (total_onshift_partners, total_busy_partners, total_outstanding_orders)

## Data Preprocessing
Handled missing values using appropriate techniques (mode/median)
Converted timestamp columns to datetime format
Created new features:
delivery_time (in minutes)
day_of_week
hour_of_day
Removed unrealistic outliers in delivery time

## Key Analysis Performed
1. Delivery Performance
Average delivery time and distribution
Outlier detection using boxplots
2. Demand Analysis
Orders by hour (peak hours identified)
Orders by day of week
3. Category and Market Insights
Delivery time across store categories
Performance comparison across markets
4. Order Characteristics
Relationship between number of items and subtotal
Weak correlation observed between order size and delivery time
5. Operational Analysis
Impact of partner availability (total_onshift_partners) and workload (total_busy_partners, total_outstanding_orders)
Higher workload leads to increased delivery time
6. Volume vs Performance
Higher order volume correlates with increased delivery time
Peak demand periods show noticeable delays

## Key Insights
Delivery delays are strongly influenced by peak hours and workload
Store category has minimal impact on delivery time
Operational factors are the primary drivers of delays
Demand spikes reduce system efficiency
Conclusion

Delivery performance is largely driven by demand and operational capacity rather than store characteristics. Optimizing partner allocation during peak hours and managing workload effectively can significantly improve delivery times and customer satisfaction.

Tools Used
Python (Pandas, Matplotlib)
Jupyter Notebook
