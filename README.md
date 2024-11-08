# Subscription_Service_Data_Analysis.

### Project Title: Subscription Service Customer Segments.
---

Table Outline
---
[Project Overview](#project-overview)

[Key Objectives](#key-objectives)

[Dataset](#dataset)

[Exploratory Data Analysis](#exploratory-data-analysis)

[Data Analysis](#data-analysis)

[Key Insights](#key-insights)

[Tools Used](#tools-used)

[Microsoft Excel](#microsoft-excel)

[SQL Queries](#sql-queries)

[PowerBI Dashboard Overview](#powerbi-dashboard-overview)

[Conclusion](#conclusion)







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

### Exploratory Data Analysis.
---
In this project, EDA was used to understood key features of the customer subscription data. The analysis covers distribution of customers segments, patterns in cancellations, and subscription trends over time. Key statistics and visualizations help identify patterns, providing insights into customer behavior and engagement. This helps inform the segmentation approach by highlighting factors associated with subscription retention and churn.









### Data Analysis.
---
- Data Cleaning and Preparation: Prepare the data for analysis by cleaning and transforming fields to ensure accuracy and consistency.
        - Checked for missing values and remove duplicates with the same values as another in all fields.
        - Converted date fields (subscriptionStart, and subscriptionEnd) to date format.
        - Created a conditional column, subscription status (Canceled) to calculate active and canceled subscription.
        - Calculated subscriptionDuration (SubscriptionStart, SubscriptionEnd) to assess the lenght of time each customer stayed subscribed.
        - Generated summary statistics such as total revenue and average subscription duration, to get a high-level view of the data.

- Calculated key Metrics;
        - Computed average subscription duration using power BI DAX functions to assess how long customers typically remain subscribed.
        - Calculated churn rate and renewal rate to understand customer retention and identify trends in cancellations.

  - Customer Segmentation: Classified customers into meaningful segments to understand the distribution and behavior across regions and subscription types.
       1. grouped customers by region and subscriptionType.
       2. Used visualizatioms to display the distribution of customer in each segment.
  - Key Findings;
       - East region have a higher concentration of active customers.
       - North, South, and West region cancellation rates are closely aligned, suggesting consistent customer behavior across these locations.
       - Basic plan has the highest retention and also churned rates, it also generated the highest revenue among other plans 
  - Revenue and Trend Analysis;
       - Analyzed total revenue by Subscription type.
       - Analyzed count of customer by subscription type and region to compare across periods to observe seasonality.
       - Used visuals (bar charts, line charts) to track subscription revenue, highlighting trends in cancellations and renewal.

   - Visualizations:
        - Created interactive power BI visuals including line charts for trends, bar charts for revenue comparisons, and cards for high-level metrics.
        - Used slicers and filters to allow exploration of data to view specific time periods and customer segments.
        
### Key Insights.
---
  - This analysis revealed significant patterns in customer subscription behaviors, preferred subscription types, and regions with high churn.
  - Active subscriptions contributed a major portion of the revenue while specific types showed higher cancellation trends, suggesting areas for potential improvement.




### Tools Used.
---
- Microsoft Excel:
      - Excel was used for initial data exploration and data cleaning tasks. Basic data manipulations; including removing duplicates, and calculated subscription duration was performed.
      - Created pivot tables to gain preliminary insights such as identifying popular subscription type, calculated basic metrics like average subscription duration, and analyzing trends in customers cancellations.
      - Also used Excel to validate calculations and compare results from SQL and Power BI, ensuring consistency.
      - Used Excel to import data into SQL database (Converted file to CSV before importing).
  
- Structured Query Language (SQL):
    - It was used for retrieval and querying; Queried data to retrieve total number of customers from each region, and created average subscription duration and total revenue by each subscription type.
   - Used to find customers who canceled their subscription within 6 months, and also customers with subscriptions longer than 12 months.
   - Used to find top 3 regions by subscription cancellations, and total number of active and canceled subscriptions.
      
- Power BI: For interactive dashboard and visualization:
   - Power BI was used for data visualization and dashboard creation, offering an interactive view of key metrics including revenue from active subscriptions and canceled subscription, average subscription duration, canceled subscription rates (Churned) and active subscription rates (Retention).
   - Implemented DAX (Data Analysis Expressions) to create calculated fields and measures such as rates of canceled and active subscriptions, allowing dynamics insights.
   - Created date table to filter and slice data by day, month, quarter, and year. This feature allowed for dynamic exploration of trends suchs as identifying peak cancellation months and track growth in subscription renewals.
   - Created conditional column to indicate active and canceled subscription to visualize more insights.
   - Created visuals (Bar charts, Line charts, and cards) to track trends over time and compare metrics across customer segments, enabling deeper analysis of subscription behavior. 


### Microsoft Excel 

Subscription Pattern.
---





<img width="540" alt="Active subscription" src="https://github.com/user-attachments/assets/e3fc6a70-d2e3-4dc4-b2b7-1857fef66d82">

This shows insights into customer subscription behavior including duration trends and popular subscription choices. As seen here we have East region leading with a count of 8,488 out of 18,612 total count which shows us that East Region has a strong potential with high customer retention, indicating an opportunity for targeted retention efforts. And also we have Basic leading in the subscriptionType gathering 11,854 out of a total of 18,612, which is indicating to us that customers prefer Basic, probably because of its low rate. Basic plan popularity, and East region should guide us around how to market, price, package, and improve the service.



The Most Popular Subscription Types by Average SubscriptionDuration.
---


<img width="299" alt="Average S  Duration pivot" src="https://github.com/user-attachments/assets/d45a8bd7-b72b-46f3-aaa2-09241793a271">

Here, Basic subsccription has accumulated the highest revenue and nearly matches the premium and standard plans in average subscription duration. This tell us that despite slight differences in duration, more customers still chose Basic plan making it the most popular option. This insights highlight opportunities to further promote the basic plan because it has strong customer base. Although as seen premium and standard have a slight longer average durations because both had 365.40 while basic has 365.30 which suggest that customers find value in all three plans but basic plan is the most preferred choice. This makes it a key focus area for the growth of the service.



Top 3 Regions with Cancellation by CustomerID and Revenue.
---


<img width="496" alt="Top 3 pivot" src="https://github.com/user-attachments/assets/03c42c2c-4af5-4f6f-a29d-3dbb3139116b">

- North, South, and West experienced the most cancellations, indicating these regions are high churn areas. It could be due to factors such as competitive offerings, i.e maybe there's a competitor offering a better offer or regional preferences or even due to economic crash affecting customer retention. And since these regions have the highest cancellation, it means that there is revenue loss so focusing on retention efforts in these areas could have meaningful impact on stabilizing revenue.
- The high number of cancellations in these regions gives an opportunity to check the cause E.g customer dissatisfaction, competitor's better offer, inflation or unmet expectations. Tailored retention strategies like targeted offers or service improvements in these regions could help reduce churn.







### SQL Queries 

Total Number of Customers Each Region.
---




<img width="424" alt="Subscription 1st requery sql" src="https://github.com/user-attachments/assets/b3add6fd-7da3-49dc-8771-ba1f42468310">


Most Popular Subscription Type by Number of Customers.
---





<img width="470" alt="Most Popular subscription SQL" src="https://github.com/user-attachments/assets/3c559ac4-ea2c-49bf-96dd-e6999d43ec50">

Customers that Canceled Subscription Within 6 Months.
---




<img width="756" alt="SQL Subscription canceled within 6 monhs newest" src="https://github.com/user-attachments/assets/c31d6414-8070-43e1-9b50-65f12a19b8a1">


Average Subscription Duration For All Customers.
---



<img width="623" alt="New Average Sub Duration" src="https://github.com/user-attachments/assets/91f4e447-fe8f-4e33-b3a1-c63615812e0f">






Customer with Subscription Longer Than 12 Months.
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


### PowerBI Dashboard Overview.
---




<img width="605" alt="Subscription Dashboard Overview NEWEST" src="https://github.com/user-attachments/assets/ee859846-9665-4917-a1ce-456c7a2f7868">







Active and Canceled Subscriptions by Region and Subscription Type.
---





<img width="340" alt="Active and Canceled Sub  by Region and Sub  Type" src="https://github.com/user-attachments/assets/86998375-ca03-4870-a915-b479b0fe551a">


Insights.
---
Active.
---
- Basic Plan: According to the visuals, Basic dominated both East region, the highest-performing region, and North region, the lowest-performing Region which made Basic the most popular plan and despite being the lowest price, it generated the highest revenue.
    - The Basic plan likely appeals to a larger customer base due to its lower price point making it an attractive option for budget-conscious users.
    - Basic plan may cover the essential features that meet the primary needs of most users which explains why it not only attracts more customers but also drives higher revenue collectively.
    - Consider upselling Basic plan users to both Premuim and Standard by offering periodic discounts or adding enticing features to both Premuim and Standard plans may attract subscribers.
    - Regular evaluation of Basic plan to ensure it remain relevant and competitive.
    - Strenghten loyalty among Basic plan users by providing exclusive content or occasional perks could drive further retention.

 - East Region:
    - East region may have higher concentration of the demographic groups E.g students, young professional or single individuals.
    - It could be as a result of part of the service offers content that is related to East region or features that are relevant to the region which may have played a significant factor in its dominance in count of customers and revenue.
    - Expanding successful localized content to other regions.
    - Conducting customer feedback surveys in this region to better understand the appeal of the service.
    - Consider region-specific content or promotions that cater to unique preferences.
      
Canceled.
---
 As seen on the visuals three regions (North, South, and West) have the same customer count with the plans (Basic, Premium, Standard) and also same revenue. The cancellation counts across all regions and plans are relatively high and close, indicating a potential issue with customer satisfaction or the perceived value of the subscriptions. 
 - Poor Customer Service Experience: Customers expect reliable and high quality service and will leave if these expectations are not met.
 - User Experience Issues: Complicated user interfaces, difficulty in navigating the service or issues with account management can frustrate users and lead them to cancel.
 - Competitor Offerings: If competitors offer better features, pricing or services, customers maybe tempted to switch. A strong competitive landscape can lead to higher cancellation rates if offerings does not keep pace.
 
 Actionable Insights.
 ---
 - Implementation of post-cancellation surveys to gather feedback from customers who cancel their subscriptions specifically ask questions about their reasons for leaving, and use this feedback to inform improvements and adjustments to offerings.
 - Improvement on customer support to proactively address issues that may lead to cancellations. E.g Offer live chat, dedicated account managers or personalized check-ins to help customers resolve problems before they decide to cancel.
 - Introduction of loyalty programs that reward customers for long-term subscriptions. E.g Offer points for renewals or incentives for referring new customers. This can enhance perceived value and encourage retention.
 - Regular evaluation and enhancement of the content and features available in the Basic, Premium, Standard plans based on customer feedback. Ensure that offerings remain competitive and relevant to customer needs.
 - Keep an eye on competitors' offerings and promotions. If they introduce features or pricing structures that attract your subscribers consider adjusting plans or marketing strategies to remain competitive.
     

Monthly Active and Canceled Subscription.
---





<img width="326" alt="Monthly Active and Canceled Sub" src="https://github.com/user-attachments/assets/22fcb947-6f55-4e82-8a96-ab569b663845">



Insights.
---
- Active Monthly Subscription: July and March have the highest count of customers with a slightly differences, this could be as a result of seasonal promotions or special offers that attract new subscribers. E.g summer promotions in July and end-of-quarter incentives in March.
   - Proactive renewal offers in these months could improve retention and make renewals more predictable.
   - Encouraging proactive engagement such as sending reminders or offering renewal discounts can sustain these peaks.

- Canceled Monthly Subscription: The cancellation trend line indicated that April has the highest canceled subscription showing that it is the weak period of customer dissatisfaction or increased competition. This might be as a result of price, low quality or irrelevant content.
   - Improvement on quality and also, introducing a discount program for long-term subscribers which could reduce price-related cancellations.
   - Introducing flexible payment options such as monthly, quarterly, and yearly payment options could improve retention price-sensitive customers. 
   - Use of user feedback to conduct monthly or quarterly surveys to understand quality concerns directly from users.
   - Regular updates to fix bugs and improve usability.
   - Introduce content recommendations base on user interests reducing irrelevant content-related cancellations.



Regional Canceled Subscriptions Revenue Over Time.
---





<img width="492" alt="Regional Canceled Sub  Revenue Over Time" src="https://github.com/user-attachments/assets/c601d80d-c6c1-4f2c-8862-adf0b35faa49">

Insights
---
According to this trend, August, 2023 has the highest cancellation revenue in West region which could be as a result of factors like holidays, end-of-summer budgeting or shifts in customer priorities; and it could be all of these stated. Economic changes or regional economic factors can also impact customers'ability or willingness to maintain subscriptions.
In this trend, we have high and low churned revenue which shows that there are factors affecting the periods either negatively or positively. What are the factors;
- Pricing Adjustments or Promotion End Dates: If a promotion or discount ended in any of these periods, some customers may have canceled after their rates returned to normal especially if the standard pricing exceeded their budget.
- Increased Competition: If a new competitor launched or intensified marketing in any of these regions and periods, customers may have opted for alternative options leading to higher cancellations.
- Customer Feedback and Dissatisfaction: If in any of these periods, there was a spike in complaints or dissatifaction, this could have led to higher cancellation rates resulting to higher churned revenue.

Actionable Insights.
---
- To combat seasonal cancellations, consider offering temporary discounts or pause options during historically high-cancellation periods to retain more customers.
- Track regional economic indicator and proactively engage customers in regions experiencing financial strain by offering flexible payment plans or short-term discounts.
- Implement a gradual increase strategy for returning to standard rates after promotions or offer alternative discounts to retain cost-sensitive customers.
- Consider launching counter-promotions or emphasizing unique features to retain subscribers during competitive launches in key regions.
    




    




Subscription Type Trend Over Time.
---



<img width="435" alt="Active Subscription Trends over time newest" src="https://github.com/user-attachments/assets/cf0a4b78-54ae-4d1b-95ec-1468afcb7112">




Insights.
---
From this visuals we can see how Basic plan dominated from January 2022 to July 2023 which is indicating that most preferred and popular plan is Basic. Factors that may have influenced this are as follows:
- Seasonal Promotions and Discounts: Promotions during the holiday seasons including discounts or a speacial deal for Basic plan may have attracted more subscribers looking for affordable options to Basic plan. E.g Summer promotional campaigns targeted at summer leisure activities may have encouraged customers to opt for the Basic plan, which may have influenced the high-rise in July 2022. 
- Increased Budget Consciousness: Given the rising cost of living, customers may have prioritized essential spending leading to a preference for the more economical Basic plan.
- End of the Year Decision-Making: As the year comes to a close, businesses and individuals often readjust their budgets and subscriptions. Customers may have chosen to switch to a Basic plan to save money heading into the new year which may have greatly influenced the high-rise on Basic plan in November 2022.
- Targeted seasonal marketing efforts emphasizing the affordability and value of the Basic plan may have successfully attracted new customers.

Actionable Insights
---
- Enhancement of Basic plan by adding seasonal content or features relevant to seasonal special offerings.
- Emphasize the Basic plan's affordability and create flexible payment options or loyalty rewards for existing customers.
- Encourage satisfied customers to share their experiences through testimonials or online reviews.
- Implement a referral program that rewards customers for referring others to the Basic plan, leveraging their positive feedback to attract new users. 

This visual above shows that Premium and Standard are not performing so well. What to do to improve customer appeal and enhance overall performance:
- Feedbacks from current and potential customers to understand their needs and reasons for not subscribing to the Premium or Standard plan and use these gathered feedbacks to improve on marketig efforts.
- Consider adjusting prices compared to competitors or implementing discounts to make these plans more attractive.
- Clearly communicate the unique benefits of the Premium and Standard plans in all marketing materials. State what differentiates these plans from the Basic plan and the provide value to customers.
- Consider offering limited-time trials for the Premium and Standard plans to allow potential customers to experience the benefits firsthand. Using this opportunity to showcase the value of these plans without financial commitment.
- Collect testimonials from satisfied customers using the Premium and Standard plans. Highlight success stories that demonstrates the value of these plans to encourage others to subscribe.

### Conclusion.
---
In conclusion, improving subscription performance requires a multifaceted approach that includes understanding customer needs, enhancing value propositions, optimizing pricing, and continously monitoring performance. By leveraging actionable insights and adapting strategies based on feedback and market conditions, the service can enhance their subscription offerings, attract new customers, and drive long-term growth.





   
