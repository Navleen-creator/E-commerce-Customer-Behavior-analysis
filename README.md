# E-commerce-Customer-Behavior-analysis
This project involves a comprehensive analysis of customer behavior for a leading eCommerce company. The analysis covers two months of data,
focusing on sales trends, traffic patterns, brand performance, and the impact of special promotions.

## Data Source
The analysis is based on two primary datasets provided by the client:
1.  **Sales_Data_Ecommerce:** Contains detailed customer behavior data including events (view, cart, purchase), pricing, categories, brands, and user sessions.
2.  **Promotion:** Contains data regarding special daily promotions featured on the app/website's first page.

## Key Business Questions Addressed
* **Pricing Trends:** Analysis of price variation by brand, category, time, and channel.
* **Traffic Analysis:** Identification of traffic patterns by day of the week, hour of the day, and platform (App vs. Browser).
* **High-Level Metrics:** Calculation of Key Performance Indicators (KPIs) including Total Revenue, Potential Revenue (cart value), and unique counts of products and categories.
* **Brand & Category Activity:** Evaluation of brand preference and activity across various parameters.
* **Search Behavior:** Exploration of how users navigate brands within categories and vice versa.
* **Promotion Impact:** Assessment of how special promotions and pricing fluctuations affect overall sales.

## Data Dictionary
### Sales_Data_Ecommerce
- `user_id`: Unique customer identifier.
- `event_date`: Date of the activity.
- `Day_of_Week`: The day the event occurred.
- `Channel`: Platform used (App/Browser).
- `event_time`/`hour`: Specific timing of the event.
- `event_type`: Action taken (view, cart, purchased).
- `product_id`/`category_id`: Unique identifiers for items and groups.
- `brand`: Brand name.
- `price`: Product price.
- `user_session`: Unique session identifier.
- `State`: Geographic location.
- `User_Score`: Customer segmentation.

### Promotions
- `Promotion Id`: Type of promotion.
- `Date`: Date of the promotion.
- `Discount`: Discount percentage.
- `ProductId`: Unique product identifier linked to the promo.

## Technical Skills Applied
- **Data Modeling:** Established relationships (Active/Inactive) between Sales, Promotions, and Calendar tables.
- **DAX Measures:** - `Total Revenue`: Sum of price for 'purchased' events.
    - `Potential Revenue`: Sum of price for 'cart' events.
    - `Total Traffic`: Distinct count of user sessions.
    - `Brand Conversion`: Ratio of purchases to total activity.
- **Data Visualization:** Matrix Heatmaps, Line Charts for trends, Slicers for interactivity, and cards

## How to Use the Dashboard
1.  **Overview Page:** Use the slicers for Brand and Channel to see how average prices fluctuate over time.
2.  **Traffic Page:** Observe the Heatmap to identify peak shopping hours.
3.  **Revenue Page:** Analyze the 'Potential Revenue' to identify opportunities for reducing cart abandonment.
