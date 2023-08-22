# Foodhub
![Cover_Image](https://github.com/Monye-Okechukwu/Foodhub/assets/136334167/d2597f13-e33a-4a39-a614-4e26aa079142)
[<sub> Source: Foodhub UNSW </sub>](https://www.eventbrite.com.au/e/food-hub-unsw-tickets-431543075957)

### Introduction
In the bustling city of New York, the restaurant scene is ever-expanding, catering to the needs of students and busy professionals who rely on convenient dining options due to their hectic lifestyles. As an answer to their culinary demands, online food delivery services have emerged as a lifeline. Among these services, FoodHub, a prominent food aggregator company, stands out by offering a singular smartphone app that provides access to a multitude of restaurants.

Through the FoodHub app, customers can place online orders directly with their preferred restaurants. Once confirmed, a designated delivery person from the company is dispatched to collect the order. Utilizing navigational tools, the delivery personnel reach the restaurant and await the food package. After receiving the order, the delivery person marks the pickup in the app and commences the journey to the customer's location, ultimately delivering the food. Following a successful delivery, the customer can rate the order using the app's interface. The business model of FoodHub involves earning revenue by retaining a fixed percentage of the delivery order's value as a commission from the restaurants.

### Objective
My task as a data scientist is to leverage the extensive order data stored in the company's online portal. By dissecting and analyzing this dataset, valuable insights can be extracted to better understand restaurant demand and subsequently enhance the overall customer experience. The Data Science team has identified crucial questions that necessitate answers for business improvement. This project involves conducting in-depth data analysis that also involve the use of statistical method like ANOVA test, MANN-WHITNEY U test, Cramer's V correlation test for the categorical data to address these inquiries, thus aiding the company in refining its operations and strategies.

### Data Description:
The dataset encompasses a variety of information pertaining to food orders and can be found [Here](https://github.com/Monye-Okechukwu/Foodhub_Analysis/blob/main/FoodHub/foodhub-order.csv). The components of the dataset are order_id, customer_id, restaurant_name, cuisine_type, cost, day_of_the_week, rating, food_preparation_time, and delivery_time. With this comprehensive dataset, an opportunity arises to dig into the intricacies of customer behavior and operational efficiency, ultimately steering the company towards informed decision-making and positive growth.

Data exploration and data visualisation was carried out using python and it can be accessed [Here](https://github.com/Monye-Okechukwu/Foodhub_Analysis/blob/main/FoodHub/FoodHub_Data_Exploration.ipynb). I also used PowerBi to create a [PowerBi Dashboard](https://app.powerbi.com/view?r=eyJrIjoiMWVlZDIyZjgtNDk2NC00YmUyLWJiZTItOGJhODExNmYzNjNhIiwidCI6ImIzNjM1MTcwLTk3MTUtNGNlNi1iMjQ0LTYxYzJkODIzMzY4ZCJ9&embedImagePlaceholder=true) and a detailed [one page report](https://github.com/Monye-Okechukwu/Foodhub_Analysis/blob/main/FoodHub/One_Page_Report.pdf).

### Conclusion and Insights
After an in-depth analysis of the Foodhub dataset, several key insights and findings have emerged:

1. **Customer Patterns:**
   - Foodhub facilitates easy online food ordering from diverse restaurants, leading to 1898 orders from 1200 customers.
   - Most customers exhibit infrequent ordering behavior, with the highest order count from a single customer being 13.
   - Top three customers eligible for 20% discount vouchers are ID 52832 (13 orders), 47440 (10 orders), and 83287 (9 orders).

2. **Restaurant Insights:**
   - The dataset covers 178 registered restaurants, with Shake Shack standing out with 219 orders.
   - American and Japanese cuisines dominate, representing 30.8% and 24.8% of orders, respectively.
   - Korean, Spanish, and Vietnamese cuisines have lower patronage, each below 15%.

3. **Order Characteristics:**
   - Order costs range from $4.47 to $35.41, with an average of $12.18. The majority of orders fall within the $10 to $15 range.
   - Weekend orders comprise 71% of total orders, and American cuisine remains popular on both weekdays and weekends.
   - Customer ratings predominantly cluster at 4 and 5, constituting over half of the total ratings.

4. **Time Metrics:**
   - Food preparation takes an average of 21 minutes, while median and mean delivery times are 25 and 24 minutes, respectively.
   - Statistical tests reveal no significant cost difference among cuisine types or food preparation times across cuisines.
   - Weekdays exhibit longer delivery times than weekends, accommodating higher order volumes.

5. **Correlations and Relationships:**
   - Positive relationships exist between order cost and food preparation time, as well as between delivery time and food preparation time.
   - A slight negative relationship is noted between delivery time and order cost.
   - Customer ID and cuisine type exhibit a medium relationship, while cuisine type and restaurant name have a strong association.
   - Four restaurants meet the criteria for promotional offers: Blue Ribbon Fried Chicken, Blue Ribbon Sushi, Shake Shack, and The Meatball Shop.

6. **Revenue Projection:**
   - Foodhub's projected revenue amounts to $6166.3 by charging 25% on orders above $20 and 15% on orders exceeding $5.

7. **Delivery Insights:**
   - Around 80.87% of orders exceed average delivery and food preparation times.
   - Approximately 10.54% of orders take over an hour for delivery.
   - The mean delivery time differs by 5 minutes and 52 seconds between weekdays and weekends.

These findings shed light on customer behavior, cuisine preferences, order dynamics, and operational efficiency within Foodhub's online food delivery service. Such insights pave the way for strategic improvements and informed decision-making, ultimately enhancing the company's services and overall business performance.

### Recommendations
Through meticulous data exploration and rigorous application of statistical methods, the following insightful recommendations have been distilled.
- Customer Ratings:
It is essential to encourage customers to give ratings for their orders. The company should emphasize the value of customer feedback and how it helps in improving the quality of service. Implementing a feedback system that incentivizes customers to rate their orders, such as offering discounts or rewards, can increase the participation rate and provide valuable insights for service improvement.

- Resource Allocation:
Since more orders were placed on weekends compared to weekdays, the company should strategically allocate additional resources during peak weekend hours. This could involve hiring extra staff, optimizing delivery routes, and ensuring efficient food preparation processes. Simultaneously, on weekdays, the company should focus on streamlining operations to ensure timely deliveries and customer satisfaction during these comparatively slower periods.

- Time Optimization:
Given that the average delivery time on weekdays is higher than on weekends, the company should identify bottlenecks in the delivery process and work towards optimizing delivery efficiency on weekdays. Similarly, the nearly similar food preparation time for weekends and weekdays should be taken advantage of by ensuring that the food preparation process is smooth and expedited during both periods to attract more customers on weekdays.

- Customer Patronage Strategy:
Identifying the customer who contributed the highest patronage presents an opportunity for the company to develop customer loyalty programs or personalized promotions for high-value customers. By recognizing and rewarding loyal customers, the company can encourage repeat business and increase customer retention.

- Cuisine Diversity:
Considering the high correlation between cuisine type and restaurant name, underperforming restaurants should explore expanding their menu to include popular cuisines like American and Japanese. This can attract a wider customer base and provide more options for customers with diverse preferences.

- Cost of Cuisines:
For cuisines such as French, Southern, Thai, and Spanish, which had higher average order costs despite lower order volumes, the company should collaborate with the respective restaurants to find ways to reduce the cost of these cuisines. Cost optimization could involve sourcing ingredients more efficiently, negotiating better deals with suppliers, or fine-tuning the menu to balance cost and customer demand.

By implementing these smart and relevant recommendations, FoodHub Company can enhance its services, improve customer satisfaction, and optimize its overall operations, leading to increased customer loyalty and business growth.
