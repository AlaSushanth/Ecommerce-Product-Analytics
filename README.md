E-Commerce Product Analytics & Conversion Optimization
📌 Project Overview

This project performs an end-to-end analysis of user behaviour on an e-commerce platform to understand how users move through the product journey and identify opportunities to improve conversion.

The analysis focuses on the customer journey:

Product View → Add to Cart → Purchase

The project investigates user behaviour, conversion drop-offs, cart abandonment, product performance, and purchase trends. Based on the insights obtained from the data, a simulated A/B testing experiment was designed to evaluate a potential product improvement.

The project combines Python, SQL, Statistical Analysis, and Power BI to demonstrate an end-to-end Product Analytics workflow.

🎯 Business Problem

An e-commerce platform receives a large number of product views, but only a small proportion of users eventually complete a purchase.

The objective of this project is to identify potential friction points in the user journey and answer the following questions:

Where do users drop off in the conversion funnel?
How many users view products, add products to the cart, and complete purchases?
What is the overall conversion rate?
What percentage of users abandon their carts?
What different types of user behaviour exist on the platform?
Which products have strong performance and which have potential for improvement?
At what times are users most likely to make purchases?
What product improvements could potentially improve conversion?
📊 Dataset

This project uses the RetailRocket E-Commerce Events Dataset.

The dataset contains user interaction events on an e-commerce platform, including:

Product Views
Add-to-Cart Events
Transactions

The key columns used in the analysis are:

Column	Description
timestamp	Time at which the event occurred
visitorid	Unique identifier for a user
event	Type of user interaction
itemid	Unique product identifier
transactionid	Transaction identifier for purchase events
Note

The raw dataset is not included in this repository because of its large file size.

🛠️ Tools & Technologies
Tool	Purpose
Python	Data cleaning, analysis and experimentation
Pandas	Data manipulation
NumPy	Numerical analysis
Matplotlib	Data visualization
Seaborn	Exploratory data visualization
SQL	Product and business analysis
Statistical Testing	Hypothesis testing and A/B test analysis
Power BI	Interactive product analytics dashboard
🔍 Analysis Performed
1. Exploratory Data Analysis

The dataset was initially explored to understand its structure and data quality.

The analysis included:

Missing value analysis
Duplicate record analysis
Unique visitor analysis
Unique product analysis
Event distribution analysis
Date range analysis

This step ensured that the dataset was properly understood before performing product-level analysis.

2. Conversion Funnel Analysis

The e-commerce user journey was analyzed using the following funnel:

View → Add to Cart → Purchase

The analysis calculates:

Total unique viewers
Users adding products to their carts
Purchasing users
View-to-Cart conversion
Overall conversion rate
Product Insight

The funnel analysis identified a substantial drop-off between the Product View and Add-to-Cart stages.

This indicates that improving the product experience at the viewing stage could potentially increase downstream conversion.

3. User Behaviour Segmentation

Users were segmented based on their interaction and purchasing behaviour.

The user segments include:

Window Shopper

Users who view products but do not complete a purchase.

Cart Abandoner

Users who add products to their cart but do not complete a purchase.

One-Time Buyer

Users who complete a single purchase.

Repeat Buyer

Users who complete multiple purchases.

This segmentation helps understand different types of platform behaviour and supports targeted product strategies.

4. Product Performance Analysis

Products were analyzed based on their interaction and conversion behaviour.

The analysis considered:

Product views
User engagement
Conversion behaviour
Product performance categories

Products were grouped into performance segments to identify:

High-performing products
Products with high visibility
Products with lower conversion
Potential product growth opportunities

This analysis helps identify products where improvements in pricing, product information, or user experience could potentially increase conversion.

5. Cart Abandonment Analysis

Cart abandonment was analyzed to understand the behaviour of users who demonstrate purchase intent but do not complete a transaction.

The analysis calculates:

Total cart users
Users abandoning their carts
Cart abandonment rate

The user journey analyzed is:

Add to Cart → No Purchase

Product Insight

Cart abandonment represents an important opportunity for conversion optimization because these users have already demonstrated stronger purchase intent compared to users who only view products.

6. Purchase Behaviour Analysis

Purchase behaviour was analyzed across different time periods.

The analysis includes:

Purchase transactions by hour
Daily purchase trends
Identification of periods with higher purchasing activity

These insights can support decisions related to:

Promotional campaign timing
Push notifications
Product launches
Marketing activities
User engagement strategies
7. SQL Analysis

A separate SQL analysis was performed to answer product and business questions using structured queries.

The SQL analysis includes areas such as:

User activity analysis
Conversion funnel analysis
Product interaction analysis
Purchase behaviour
User segmentation
Cart abandonment

The SQL analysis is maintained in a separate notebook to demonstrate independent SQL analytical capability.

8. Statistical Hypothesis Testing

Statistical hypothesis testing was performed to evaluate behavioural patterns identified during the analysis.

The process included:

Defining the Null Hypothesis
Defining the Alternative Hypothesis
Selecting an appropriate statistical test
Calculating the test statistic
Calculating and interpreting the p-value
Making a data-driven conclusion
🧪 9. Simulated A/B Testing
Business Problem

The conversion funnel identified a significant drop-off between:

Product View → Add to Cart

Based on this insight, a simulated product experiment was designed to evaluate whether an improved product page could increase the Add-to-Cart conversion rate.

Important: The original RetailRocket dataset does not contain actual Control and Treatment group assignments. Therefore, this section represents a simulated A/B testing case study based on insights obtained from the dataset.

Experiment Design
Control Group

Users experience the existing product page.

Treatment Group

Users experience an improved product page with:

More prominent Add-to-Cart button
Clearer product information
Improved product presentation
Primary Metric

Add-to-Cart Conversion Rate

Add-to-Cart Conversion Rate = Users Adding to Cart / Product Viewers

Hypotheses
Null Hypothesis (H₀)

The improved product page does not improve the Add-to-Cart conversion rate.

Alternative Hypothesis (H₁)

The improved product page improves the Add-to-Cart conversion rate.

Statistical Test

A Two-Proportion Z-Test was performed to compare the conversion rates of the Control and Treatment groups.

The simulated experiment results showed that:

The Treatment group achieved a higher conversion rate.
The statistical test produced a p-value below the selected significance level.
The Null Hypothesis was rejected.
Conclusion

Reject the Null Hypothesis. The treatment shows a statistically significant improvement in the Add-to-Cart conversion rate.

Product Recommendation

Based on the simulated experiment, the improved product page could be rolled out to a larger user population while continuing to monitor:

Add-to-Cart Conversion
Purchase Conversion
Cart Abandonment
Downstream user behaviour
📈 Power BI Dashboard

An interactive Power BI dashboard was developed to present the key product analytics insights.

The dashboard consists of five pages.

Page 1: Executive Overview

Provides a high-level overview of key product metrics.

Metrics include:

Unique Viewers
Users Adding to Cart
Purchasing Users
Overall Conversion Rate
Conversion Funnel
Page 2: User Behaviour & Segmentation

Analyzes user behaviour across different segments.

Includes:

User Segment Distribution
Number of Users by Segment
Purchase Transactions by Hour
Page 3: Product Performance

Analyzes how products perform across different performance segments.

Includes:

Product Performance Matrix
Number of Products by Performance Segment
Page 4: Cart Abandonment Analysis

Tracks important cart-related metrics.

Includes:

Total Cart Users
Users Who Abandoned Cart
Cart Abandonment Rate
Page 5: Purchase Trends & Insights

Analyzes purchasing patterns over time.

Includes:

Purchase Transactions by Hour
Daily Purchase Trends
💡 Key Product Insights
1. Improve View-to-Cart Conversion

A large number of users interact with products without adding them to their carts.

Potential improvements include:

Improving product page design
Providing clearer product information
Improving pricing visibility
Optimizing Call-to-Action placement
Improving personalized recommendations
2. Reduce Cart Abandonment

Users who add products to their cart have demonstrated stronger purchase intent.

Potential interventions include:

Simplifying checkout
Displaying delivery information earlier
Reducing unexpected costs
Sending cart reminders
Improving payment flow
3. Focus on High-Potential Products

Products with high visibility but lower conversion can be investigated further.

Potential causes include:

Pricing
Product information
User experience
Product availability
Purchase friction
4. Use Segment-Specific Strategies

Different user groups require different product interventions.

User Segment	Potential Product Strategy
Window Shopper	Improve product discovery and recommendations
Cart Abandoner	Cart reminders and checkout optimization
One-Time Buyer	Post-purchase engagement
Repeat Buyer	Loyalty and retention initiatives
🚀 Final Product Recommendations

Based on the analysis, the following product actions are recommended:

Improve Product Page Experience

Optimize product information and Call-to-Action visibility to improve View-to-Cart conversion.

Reduce Checkout Friction

Simplify the checkout process and reduce unexpected costs that may contribute to cart abandonment.

Prioritize High-Potential Products

Investigate products with high user engagement but lower conversion to identify potential friction points.

Use Behaviour-Based Targeting

Develop different engagement strategies for Window Shoppers, Cart Abandoners, One-Time Buyers, and Repeat Buyers.

Validate Product Changes Through Experimentation

Use controlled experiments and A/B testing to measure the impact of product changes before a large-scale rollout.

📂 Project Structure
Ecommerce-Product-Analytics/
│
├── notebooks/
│   ├── Ecommerce_Product_Analytics_Python.ipynb
│   └── Ecommerce_Product_Analytics_SQL.ipynb
│
├── dashboard/
│   └── Ecommerce_Product_Analytics_Dashboard.pbix
│
├── images/
│   ├── executive_overview.png
│   ├── user_behaviour.png
│   └── product_performance.png
│
└── README.md
🎯 Key Skills Demonstrated
Product Analytics
Funnel Analysis
Conversion Analysis
User Behaviour Analysis
User Segmentation
Product Performance Analysis
Cart Abandonment Analysis
SQL
Python
Exploratory Data Analysis
Statistical Hypothesis Testing
Two-Proportion Z-Test
A/B Testing Framework
Power BI Dashboard Development
Business Insights
Product Recommendations
🔮 Future Improvements

Potential future extensions include:

Cohort retention analysis
Customer lifetime value analysis
Customer journey analysis
Predictive conversion modelling
Real-world A/B test analysis
Recommendation system analysi
