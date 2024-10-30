# Subscription_Service_Data_Analysis.

### Project Title: Subscription Service Customer Segments.
---

### Project Overview.
---
This project aims to analyze customer behaviour for a subscription-based service, focusing on identifying customer segments, tracking subscription trends, and understanding cancellation patterns. By gaining insights into these areas, the analysis helps to uncover patterns that could inform strategies to improve customer retention and tailor marketing efforts. 

### Key Objectives.
---
1. Customer Segmentation: Classify customers by region, subscription type, and activity status to understand who the primary customer segments are.

2. Cancellation Analysis: Examine cancellation patterns by region and subscription type to determmine where and why customers are leaving.

3. Subscription Trends: Track monthly trends in active vs canceled customers to reveal insights into seasonal behaviors and subscription life cycle stages.

### Dataset.
---
The dataset used includes customer data with the following fields: 
  - CustomerID: Unique identifier for each customer on this dataset. 
  - CustomerName: Name of each customer who subscribed to the service.
  - Region: Geographical location of customers who subscribed to the service
  - SubscriptionType: This is the type of subscription each customer subscribed to.
  - SubscriptionStart: This is date customer subscription start. 
  - SubscriptionEnd: It is the date customer subscription ends.
  - Canceled: This to know which customer canceled his or her subscription.
  - Revenue: This the the total amount of money generated.

### Data Analysis.
---
- Data Cleaning and Preparation: Prepare the data for analysis by cleaning and transforming fields to ensure accuracy and consistency.
      1. Checked for missing values and remove duplicates with the same values as another in all fields.
      2. Converted date fields (subscriptionStart, and subscriptionEnd) to date format.
      3. Created a conditional column, subscription status to calculate active and canceled subscription.
      4. Calclated subscriptionDuration to assess the lenght of time each customer stayed subscribed.
  Now, data was cleaned and ready for further analysis, with calculated fields added for segmentation and trend tracking.

  - Customer Segmentation: Classified customers into meaningful segments to under




### Tool Used.
---
- Microsoft Excel:
- Structured Query Language (SQL): For data query and EXtraction.
- Power BI: For interactive dashboard and visualization.

### Key Insights.
---
- Identification of high-cancellation regions and subscription types.
- Monthly 






















