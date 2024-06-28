# Smart Shopper Profiling System Using RFM-T

Image Sources: Pexels.com
In today's digital era, e-commerce faces the challenge of understanding and optimizing their customer experience. The main issue at hand is how to effectively profile customers based on their transaction frequency and spending amount. With a variety of customer information such as demographic data, shopping habits, and feedback, companies need to analyze this data in depth to identify patterns and trends that can help improve their business strategies. Without proper analysis, e-commerce risks missing out on opportunities to increase customer loyalty, personalize offers, and better manage inventory.

The "Smart Shopper Profiling System Using RFM-T" project aims to profile e-commerce customers based on transaction activity or how frequently they shop and the amount spent using RFM-T (Recency, Frequency, Monetary, Tenure). This goal is achieved by identifying three distinct customer segments, allowing companies to optimize marketing and customer service strategies. The solution provides a holistic view of customer behavior, enabling companies to develop more effective marketing strategies, improve customer service, and ultimately drive customer growth and loyalty. With comprehensively analyzed data, companies can make better and informed decisions to optimize their retail operations.
https://www.kaggle.com/datasets/bhavikjikadara/retail-transactional-dataset/data

**📃 Data:**

|       | **Attribute**          | **Information**                                                 |
| :---  | :--------------------- | :-------------------------------------------------------------- |
| **1** | **Transaction ID**     | Unique ID of the transaction                                    |
| **2** | **Customer ID**        | Unique ID of the customer (Primary key)                         |
| **3** | **Name**               | Name of the customer                                            |
| **4** | **Email**              | Email address                                                   |
| **5** | **Phone**              | Contact number                                                  |
| **6** | **Address**            | Address                                                         |
| **7** | **City**               | City                                                            |
| **8** | **State**              | State                                                           |
| **9** | **Zipcode**            | Postal code                                                     |
| **10**| **Country**            | Country                                                         |
| **11**| **Age**                | Age                                                             |
| **12**| **Gender**             | Gender                                                          |
| **13**| **Income**             | Income level                                                    |
| **14**| **Date**               | Date of the last transaction                                    |
| **15**| **Year**               | Year of the transaction                                         |
| **16**| **Month**              | Month of the transaction                                        |
| **17**| **Time**               | Time of the transaction                                         |
| **18**| **Total Purchases**    | Total number of purchases made by the customer                  |
| **19**| **Amount**             | Amount of money spent in a single transaction                   |
| **20**| **Total Amount**       | Total amount of money spent by the customer                     |
| **21**| **Product Category**   | Category of the product purchased (e.g., electronics, clothing, groceries) |
| **22**| **Product Brand**      | Brand of the product purchased                                  |
| **23**| **Product Type**       | Type or model of the product purchased                          |
| **24**| **Feedback**           | Customer feedback or rating regarding the product or service received |
| **25**| **Shipping Method**    | Method used to ship the purchased product                       |
| **26**| **Payment Method**     | Payment method used                                             |
| **27**| **Order Status**       | Order status (e.g., shipped, received, canceled)                |
| **28**| **Ratings**            | Customer rating of the product or service                       |
| **29**| **Products**           | List of products purchased                                      |


## Data Preprocessing:
- **Data Wrangling**
    - **Missing Values**
    - **Duplicate**
    - **Inconsistent**
- **Outliers**
- **Feature Engineering**
	- determine features that are not redundant, and most logical

## Modeling:
- **RFMT**
- Scaling
- Clustering RFMT with K-Means, utilizing additional data (Total Product and Ratings).

What is used when RFMT:
1. Customer_ID
2. Transaction_ID
3. Total_Amount
4. Time = `Date` + `Time` (format datetime64[ns])

## Evaluation:
- Evaluate each k using silhouette coefficient and Calinski-Harabasz index.
- The final clustering with the best k resulted in three clear segments.
- Profiling shows the unique characteristics of each cluster.


## Conclusion:
This project successfully identified three distinct customer segments:

1. "Dormant Long-term Customers": Requires reactivation strategy.
2. "Emerging Potential Shoppers": Focus on developing and increasing value.
3. "High-Value Active Enthusiasts": Priority on retention and value maximization.

Main Insights:
1. Strong correlation seen between frequency, monetary value, and total products. Customers who shop frequently tend to spend more money and buy more products.
2. Tenure has a positive correlation with frequency and monetary value, suggesting long-standing customers tend to be more valuable.
3. Recency is negatively correlated with frequency and monetary value, indicating customers who have recently shopped tend to be more active and valuable.
4. Ratings show no clear pattern in distinguishing clusters, indicating customer satisfaction may not always correlate with purchase behavior.

Recommendation:
1. Implementation of personalization strategies for each segment.
    - Dormant Long-term Customers: Send personalized emails with special offers or exclusive discounts to attract them back. For example, give a 20% discount on a product they have frequently purchased before.
    - Emerging Potential Shoppers: Offer product recommendations based on their purchase history and invite them to subscribe to the newsletter to get information about new products and exclusive offers.
    - High-Value Active Enthusiasts: Provide access to exclusive products before they are launched to the general market and invite them to participate in loyalty programs with attractive rewards.
---

2. Focus on increasing engagement for "Dormant Long-term Customers".
    - Send email campaigns asking why they stopped shopping and offer incentives to provide feedback.
    - Hold contests or sweepstakes with attractive prizes that encourage them to return.
---

3. Special development program for "Emerging Potential Shoppers".
    - Offer exclusive memberships with benefits such as discounts, early access to sales, and special events.
    - Create a referral program that encourages them to invite friends and family to shop on your platform.
---

4. Exclusive reward and loyalty programs for "High-Value Active Enthusiasts".
    - Give reward points for every purchase that can be redeemed for discounts or free products.
    - Invite them to join a VIP program with access to exclusive offers, special events and priority customer service.
---

5. Enhance customer experience to increase the correlation between ratings and purchase behavior.
    - Improve customer service with quick responses to complaints and inquiries.
    - Conduct regular customer satisfaction surveys and use the feedback to improve product and service quality.

------------------------------------------------------------------------
