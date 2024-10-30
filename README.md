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

  - Customer Segmentation: Classified customers into meaningful segments to understand the distribution and behavior across regions and subscription types.
       1. grouped customers by region and subscriptionType.
       2. Used visualizatioms to display the distribution of customer in each segment.
  - Key Findings;
       - Cert




### Tool Used.
---
- Microsoft Excel:
- Structured Query Language (SQL): For data query and EXtraction.
- Power BI: For interactive dashboard and visualization.

### Key Insights.
---
- Identification of high-cancellation regions and subscription types.
- Monthly trends visualization for active and canceled subscriptions, revealing peak and off-peak seasons.
- Customer segmentation that highlight

### Microsoft Excel 

Subscription Pattern.
---





<img width="540" alt="Active subscription" src="https://github.com/user-attachments/assets/e3fc6a70-d2e3-4dc4-b2b7-1857fef66d82">

The Most Popular Subscription Types by Average SubscriptionDuration.
---





<img width="299" alt="Average S  Duration pivot" src="https://github.com/user-attachments/assets/d45a8bd7-b72b-46f3-aaa2-09241793a271">


Top 3 
---




<img width="496" alt="Top 3 pivot" src="https://github.com/user-attachments/assets/03c42c2c-4af5-4f6f-a29d-3dbb3139116b">

### SQL Queries 

Total Number of Customers Each Region.
---




<img width="424" alt="Subscription 1st requery sql" src="https://github.com/user-attachments/assets/b3add6fd-7da3-49dc-8771-ba1f42468310">

Most Popular Subscription Type by Number of Customers.
---





<img width="470" alt="Most Popular subscription SQL" src="https://github.com/user-attachments/assets/3c559ac4-ea2c-49bf-96dd-e6999d43ec50">

Customers that Canceled Subscription Within 6 Months.
---






Average Subscription Duration For All Customers.
---





<img width="652" alt="Average subscription duration subscription" src="https://github.com/user-attachments/assets/f3e83a99-475a-4532-9f03-bd3328ff87b0">

Customer With Subscription Longer Than 12 Months.
---



<img width="660" alt="sub longer than 12 months" src="https://github.com/user-attachments/assets/669bc791-f241-410a-9973-a223899b1f83">

Total Revenue by Subscription Type.
---





<img width="569" alt="Total revenue subscription type" src="https://github.com/user-attachments/assets/e372689f-c642-4329-8f4d-9c4facafdf31">

Top 3 Regions by Subscription Cancellations.
---





<img width="628" alt="Top 3 regions subscription sql" src="https://github.com/user-attachments/assets/ded7c124-bf8a-465a-9003-e86743cf6e55">

Total Number of Active and Canceled Subscriptions.
---





<img width="628" alt="Total active and canceled sub sql" src="https://github.com/user-attachments/assets/4c123a43-84bf-4f94-b757-9c0d1748c028">






