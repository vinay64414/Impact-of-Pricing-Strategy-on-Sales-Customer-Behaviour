# Impact-of-Pricing-Strategy-on-Sales-Customer-Behaviour
Analyzed e-commerce sales data to understand how pricing and discount strategies influence revenue, profit, sales volume, and customer behavior. Built interactive Tableau visualizations to compare discount levels, product categories, regions, seasons, and customer segments, turning raw data into actionable business insights.
# Impact of Pricing Strategy on Sales and Customer Behaviour

## 📌 Project Overview

Pricing plays an important role in determining sales, revenue, profitability, and customer purchasing behaviour. A discount may encourage customers to purchase more, but excessive discounting can reduce profit and even result in loss-making transactions.

This project analyzes an e-commerce sales dataset to understand how **pricing and discount strategies influence sales performance, profitability, and customer behaviour**.

The project combines **Python, SQL, and Tableau** to move from raw data to meaningful business insights and interactive visualizations.

The analysis focuses on questions such as:

- How do different discount levels affect revenue?
- Does a higher discount increase quantity sold?
- At what discount level does profitability start declining?
- Which product categories generate the most revenue?
- Which regions generate the highest profit?
- Which customer groups contribute more to revenue?
- How do seasonal and monthly patterns affect sales?
- Are there transactions where excessive discounts result in negative profit?

---

## 🎯 Project Objectives

The main objectives of this project are:

1. Analyze the relationship between pricing, discounts, revenue, and profit.
2. Identify the impact of discounts on customer purchasing behaviour.
3. Compare revenue and profitability across product categories.
4. Analyze customer behaviour based on age and gender.
5. Identify regional differences in sales and profitability.
6. Understand monthly and seasonal sales patterns.
7. Identify loss-making transactions.
8. Segment customers based on their purchasing value.
9. Develop business hypotheses and validate them using SQL.
10. Build interactive dashboards to communicate the findings clearly.
11. Provide actionable recommendations for better pricing decisions.

---

# 📂 Dataset

The dataset contains e-commerce transaction-level information.

### Dataset Columns

| Column | Description |
|---|---|
| `Order_ID` | Unique identifier for each order |
| `Customer_ID` | Identifier of the customer |
| `Product_ID` | Identifier of the product |
| `Category` | Product category |
| `Original_Price` | Product price before discount |
| `Discount_Percent` | Discount percentage applied to the product |
| `Quantity` | Number of units purchased |
| `Order_Date` | Date on which the order was placed |
| `Final_Price` | Price after applying the discount |
| `Cost` | Cost associated with the product |
| `Customer_Age` | Age of the customer |
| `Customer_Gender` | Gender of the customer |
| `Region` | Customer's broad geographical region |
| `Payment_Method` | Payment method used for the transaction |
| `Month` | Month of the transaction |
| `Adjusted_Revenue` | Revenue value used for analysis |
| `Revenue_Check` | Revenue calculation/check field |
| `Profit_Check` | Profit calculation/check field |
| `Season` | Seasonal classification of the transaction |

---

# 🛠️ Tools & Technologies

### Python
Used for data cleaning, exploratory data analysis, statistical analysis, and identifying patterns.

Libraries used:

- Pandas
- NumPy
- Matplotlib
- Seaborn

### SQL / MySQL
Used for:

- Business hypothesis testing
- Customer analysis
- Category analysis
- Regional analysis
- Pricing analysis
- Aggregations
- Group-based comparisons

### Tableau
Used to create interactive dashboards and visualizations for business storytelling.

---

# 🔄 Project Workflow

```text
Raw Dataset
     ↓
Data Understanding
     ↓
Data Cleaning & Validation
     ↓
Exploratory Data Analysis using Python
     ↓
Statistical Analysis
     ↓
Business Hypothesis Development
     ↓
SQL Analysis
     ↓
Interactive Tableau Visualizations
     ↓
Business Insights
     ↓
Actionable Recommendations


1. Exploratory Data Analysis Using Python

Python was used to understand the structure and behaviour of the dataset before creating the dashboards.

The analysis included:

Dataset structure
Data types
Missing values
Descriptive statistics
Revenue distribution
Profit distribution
Discount analysis
Correlation analysis
Covariance analysis
Skewness and kurtosis
Outlier detection
Loss-making transactions
Customer-level analysis
Category-level analysis
Regional analysis
Seasonal analysis
📊 2. Descriptive Statistics
Revenue Statistics

The analysis produced the following revenue statistics:

Mean Revenue: ₹2,324.15
Median Revenue: ₹1,876.74
Mode Revenue: ₹2,202.84

The mean revenue is higher than the median, indicating that some higher-value transactions are pulling the average upward.

This suggests that most transactions are relatively lower in value, while a smaller number of high-value transactions contribute significantly to total revenue.

📈 3. Revenue Variability

The following statistics were analyzed:

Variance: 2,907,592.24
Standard Deviation: 1,705.17
Range: ₹8,247.98

The relatively large standard deviation indicates that transaction revenues vary considerably.

This means customers do not spend the same amount per transaction. Some transactions are considerably larger than others.

This is useful for identifying different customer value groups and developing targeted marketing strategies.

📐 4. Distribution Analysis
Skewness

Skewness: 0.843

The positive skewness indicates that the revenue distribution is right-skewed.

In simple terms:

There are more lower-value transactions and fewer high-value transactions.

This suggests that the business has a larger base of lower-spending customers along with a smaller group of high-spending customers.

Business Use

This can support customer segmentation strategies such as:

Low-value customers → targeted promotions
Medium-value customers → cross-selling and upselling
High-value customers → loyalty and premium offers
📊 5. Correlation Analysis

Correlation analysis was performed between important pricing, sales, and profitability variables.

Some important relationships were:

Relationship	Correlation
Revenue vs Profit	0.982
Profit vs Quantity	0.687
Revenue vs Quantity	0.589
Revenue vs Final Price	0.739
Discount vs Profit	-0.165
Discount vs Revenue	-0.141
Key Insight

Revenue and profit have a very strong positive relationship.

Quantity also has a positive relationship with revenue and profit, suggesting that selling more units generally contributes to higher revenue and profitability.

However, discount percentage has a negative relationship with profit.

This supports an important project hypothesis:

Increasing discounts may encourage sales, but excessive discounting can put pressure on profitability.

💰 6. Pricing & Discount Analysis

Pricing strategy is the central theme of this project.

The analysis follows this relationship:

Original Price
      ↓
Discount
      ↓
Final Price
      ↓
Quantity Purchased
      ↓
Revenue
      ↓
Profit

The project investigates whether increasing discounts actually creates enough additional sales volume to compensate for the reduction in selling price.

🎯 Discount Band Analysis

To make the discount analysis easier to understand, discounts can be grouped into bands such as:

0%
5%
10%
15%
20%
25%
30%
...
80%

This makes it easier to compare revenue and profitability at different discount levels.

Key Questions
Which discount level generates the highest revenue?
Which discount level generates the highest quantity?
Which discount levels reduce profitability?
Does a higher discount always produce higher sales?
Which category performs best at each discount level?
📦 7. Category Analysis

Average revenue by category:

Category	Average Revenue
Clothing	₹2,416.14
Beauty	₹2,327.36
Home	₹2,279.57
Electronics	₹2,263.14
Insight

Clothing has the highest average revenue among the categories, while Electronics has the lowest average revenue.

However, revenue alone should not determine the pricing strategy.

Profit and profit margin should also be considered before deciding which categories should receive additional discounts or promotional investment.

🌍 8. Regional Analysis

Total profit by region:

Region	Total Profit
West	₹10.02M
South	₹9.75M
East	₹8.59M
North	₹7.73M
Key Insight

The West region generates the highest total profit, followed closely by the South.

The North region generates the lowest total profit among the four regions.

This suggests that pricing and promotional strategies could potentially be adjusted according to regional performance.

👥 9. Customer Behaviour Analysis

The dataset contains approximately 100 unique customers, with Customer IDs ranging from 1000 to 1099.

Because customers appear across multiple transactions, repeat purchasing behaviour can be analyzed.

Customer-level statistics include:

Total revenue per customer
Average transaction revenue
Number of purchases

Example:

Customer	Total Revenue	Avg Revenue	Purchases
1000	₹928,004.47	₹2,643.89	351
1001	₹639,634.67	₹2,118.00	302
1002	₹709,565.31	₹2,750.25	258
Customer Segmentation

Customers can be divided into:

Low Value
Medium Value
High Value

This allows the business to develop different strategies for different customer groups.

🎯 10. Customer Segmentation Strategy
Low-Value Customers

Possible strategies:

Entry-level discounts
Product recommendations
First/next purchase incentives
Bundle offers
Medium-Value Customers

Possible strategies:

Cross-selling
Upselling
Category recommendations
Personalized promotions
High-Value Customers

Possible strategies:

Loyalty programs
Premium offers
Exclusive discounts
Early access to products

The objective is to increase customer lifetime value rather than simply giving discounts to everyone.

🚻 11. Gender-Based Analysis

Average revenue by gender was also analyzed.

Gender	Average Revenue
Female	₹2,321.72
Male	₹2,326.51

The difference is relatively small.

Therefore, gender alone may not be a strong indicator of spending behaviour in this dataset.

Instead, gender can be combined with:

Category
Age
Region
Discount
Revenue

to identify more meaningful purchasing patterns.

👤 12. Age-Based Customer Behaviour

Customer age can be used to investigate:

Which age groups purchase more?
Which age groups receive higher discounts?
Which age groups generate higher revenue?
Which categories are preferred by different age groups?

Possible customer groups:

Young Customers
Middle-Age Customers
Older Customers

These groups can then be compared based on:

Average revenue
Quantity
Discount
Category preference
📅 13. Monthly Revenue Analysis

Monthly revenue:

Month	Revenue
January	₹4.89M
February	₹4.43M
March	₹5.11M
April	₹5.07M
May	₹4.09M
June	₹4.49M
July	₹5.20M
August	₹4.31M
September	₹3.88M
October	₹4.00M
November	₹2.98M
December	₹2.68M
Key Insight

July generated the highest monthly revenue, while December generated the lowest.

This can be investigated further to determine whether pricing, discount levels, seasonality, product mix, or customer behaviour contributed to these differences.

🍂 14. Seasonal Analysis

Average profit:

Season	Average Profit
Festive	₹1,735.46
Regular	₹1,619.65
Insight

Festive periods generate higher average profit than regular periods.

This suggests that customers may be more willing to purchase during festive periods, creating an opportunity to use targeted promotions without relying on extremely high discounts.

⚠️ 15. Outlier Detection

The Interquartile Range (IQR) method was used to detect unusual revenue transactions.

Result

Number of revenue outliers: 136

These transactions may represent:

Very high-value orders
Unusual quantities
Premium products
Special pricing
Exceptional customer purchases

Outliers should not automatically be removed because they may contain valuable business information.

❗ 16. Loss-Making Transactions

One of the most important findings from the analysis was the presence of negative-profit transactions.

Original Result

Loss-making transactions: 298

Example transactions included:

Category	Discount	Profit
Electronics	30%	-₹63.69
Home	30%	-₹30.17
Home	30%	-₹124.83
Electronics	30%	-₹50.61
Possible Reasons

Negative profit may occur because of:

High discount
High product cost
Low final selling price
Pricing that does not sufficiently cover cost
🚨 17. Discount Simulation

A pricing simulation was performed to investigate the impact of a discount rule.

The original number of loss-making transactions was:

298

After applying the simulated pricing condition, the resulting loss count was:

1,503

This result highlights the importance of carefully validating a pricing rule before implementing it.

A pricing strategy should not simply be judged by whether it increases sales volume.

It should also be evaluated based on:

Revenue
Profit
Profit margin
Quantity
Loss-making transactions
🧪 18. SQL Hypothesis Analysis

SQL was used to test business hypotheses derived from the Python analysis.

Hypothesis 1

Do higher discounts increase revenue?

SELECT 
    Discount_Percent,
    SUM(Adjusted_Revenue) AS Total_Revenue
FROM sales
GROUP BY Discount_Percent
ORDER BY Discount_Percent;
Hypothesis 2

Do higher discounts increase sales volume?

SELECT 
    Discount_Percent,
    SUM(Quantity) AS Total_Quantity
FROM sales
GROUP BY Discount_Percent
ORDER BY Discount_Percent;
Hypothesis 3

Do higher discounts reduce profitability?

SELECT 
    Discount_Percent,
    SUM(Profit_Check) AS Total_Profit
FROM sales
GROUP BY Discount_Percent
ORDER BY Discount_Percent;
Hypothesis 4

Which categories generate the highest revenue?

SELECT 
    Category,
    SUM(Adjusted_Revenue) AS Total_Revenue
FROM sales
GROUP BY Category
ORDER BY Total_Revenue DESC;
Hypothesis 5

Which regions generate the highest profit?

SELECT 
    Region,
    SUM(Profit_Check) AS Total_Profit
FROM sales
GROUP BY Region
ORDER BY Total_Profit DESC;
Hypothesis 6

Which customers purchase from multiple categories?

SELECT 
    Customer_ID,
    COUNT(DISTINCT Category) AS Category_Count
FROM sales
GROUP BY Customer_ID
HAVING COUNT(DISTINCT Category) > 1;
Hypothesis 7

Which payment methods generate the most revenue?

SELECT 
    Payment_Method,
    SUM(Adjusted_Revenue) AS Total_Revenue
FROM sales
GROUP BY Payment_Method
ORDER BY Total_Revenue DESC;
📊 19. Tableau Dashboard

The final stage of the project is an interactive Tableau dashboard designed around the project title.

Dashboard 1 — Pricing Strategy Overview
Recommended KPIs
Total Revenue
Total Profit
Average Discount
Total Quantity
Total Orders
Recommended Visualizations

Discount vs Revenue

Columns → Discount_Percent
Rows → SUM(Adjusted_Revenue)
Color → Category
Size → SUM(Quantity)

Purpose:

Understand how different discount levels influence revenue across categories.

Discount vs Profit
Columns → Discount_Percent
Rows → SUM(Profit_Check)
Color → Category

Purpose:

Identify discount levels where profitability starts declining.

Dashboard 2 — Customer Behaviour

Recommended visualizations:

Customer Spending
Columns → Customer_Age
Rows → SUM(Adjusted_Revenue)
Color → Customer_Gender
Gender vs Category
Columns → Category
Rows → SUM(Quantity)
Color → Customer_Gender
Customer Segment
Columns → Customer Segment
Rows → SUM(Adjusted_Revenue)

Purpose:

Understand who the customers are, what they buy, and how much they spend.

🌍 Dashboard 3 — Regional & Category Performance

Recommended visualizations:

Region-wise Revenue
Columns → Region
Rows → SUM(Adjusted_Revenue)
Color → SUM(Profit_Check)
Category Revenue
Columns → Category
Rows → SUM(Adjusted_Revenue)
Category Profit
Columns → Category
Rows → SUM(Profit_Check)

Purpose:

Identify high-performing and underperforming markets and categories.

📅 Dashboard 4 — Time & Seasonality
Monthly Revenue Trend
Columns → Month
Rows → SUM(Adjusted_Revenue)
Color → Season
Seasonal Profit
Columns → Season
Rows → AVG(Profit_Check)

Purpose:

Identify peak periods and understand when pricing and promotional strategies may be most effective.

📌 Key Business Insights

The analysis produced several important findings:

1. Revenue is right-skewed

Most transactions are relatively lower in value, while a smaller number of high-value transactions contribute significantly to the overall revenue.

2. Discounts need to be optimized

Discounting can influence purchasing behaviour, but excessive discounts can negatively affect profitability.

3. Revenue and profit are strongly connected

The high positive correlation between revenue and profit indicates that higher-value transactions generally contribute strongly to profitability.

4. Quantity is an important driver

Quantity has a positive relationship with both revenue and profit.

5. Clothing has the highest average revenue

Clothing recorded the highest average transaction revenue among the categories.

6. West generates the highest total profit

The West region has the highest total profit among the four regions.

7. Festive periods perform better

Average profit during festive periods is higher than during regular periods.

8. Loss-making transactions require attention

The existence of negative-profit transactions highlights the need for pricing controls.

9. Customer segmentation can improve marketing

Different customer value groups can be targeted with different promotional and retention strategies.

💡 Business Recommendations

Based on the analysis, the following recommendations can be considered:

💰 1. Avoid blanket discounts

Instead of providing the same discount to every customer or product, use targeted discounts based on:

Customer value
Product category
Region
Season
Purchase behaviour
📊 2. Establish safe discount ranges

Identify discount levels that provide a reasonable balance between:

Sales Volume + Revenue + Profit
🛍️ 3. Promote profitable categories

Categories that generate strong revenue and profit should receive strategic promotional support.

👥 4. Focus on customer retention

Repeat customers can be targeted through:

Loyalty programs
Personalized offers
Product recommendations
Cross-selling
Upselling
🌍 5. Use regional pricing strategies

Different regions show different profitability levels.

Pricing and promotions can therefore be adjusted based on regional performance.

📅 6. Use seasonal pricing

Higher-performing periods can be used for strategic promotions, while weaker periods can use targeted incentives to stimulate demand.

⚠️ 7. Monitor loss-making transactions

Transactions generating negative profit should be regularly monitored.

Products with:

High cost
High discount
Low final price

should be reviewed before additional discounts are offered.

📈 Project Outcome

This project demonstrates how raw e-commerce transaction data can be transformed into actionable business intelligence.

The combination of:

Python
   +
SQL
   +
Tableau
   ↓
Business Insights
   ↓
Pricing Recommendations

helps connect technical data analysis with real-world business decision-making.

The final dashboard provides an interactive view of:

Pricing strategy
Discount effectiveness
Revenue
Profitability
Customer behaviour
Category performance
Regional performance
Seasonal trends
🧠 Skills Demonstrated
Data Cleaning
Exploratory Data Analysis
Statistical Analysis
Data Validation
Correlation Analysis
Covariance Analysis
Outlier Detection
Customer Segmentation
Business Hypothesis Testing
SQL Aggregations
GROUP BY / HAVING
Revenue & Profit Analysis
Pricing Strategy Analysis
Data Visualization
Tableau Dashboard Development
Business Storytelling
Actionable Recommendations
📁 Suggested Repository Structure
Impact-of-Pricing-Strategy-on-Sales-and-Customer-Behaviour/
│
├── README.md
│
├── data/
│   └── sales_dataset.csv
│
├── python/
│   └── EDA_Pricing_Strategy.ipynb
│
├── sql/
│   └── Business_Hypotheses.sql
│
├── tableau/
│   └── Pricing_Strategy_Dashboard.twbx
│
├── dashboard/
│   └── dashboard_screenshot.png
│
└── presentation/
    └── Business_Insights.pdf
🚀 Future Scope

The project can be extended with machine learning and advanced analytics.

Potential future improvements include:

Customer Lifetime Value prediction
Sales forecasting
Customer churn prediction
Demand prediction
Price elasticity analysis
Optimal discount prediction
Customer clustering using machine learning
Product recommendation systems
Predictive pricing models

These extensions can help move the project from descriptive analytics toward predictive and prescriptive analytics.

🏁 Conclusion

The project shows that pricing decisions should not be evaluated only by looking at sales or revenue.

A discount may increase purchasing activity, but the real business question is:

Does the additional sales volume generated by the discount create enough revenue and profit to justify the price reduction?

By combining Python-based analysis, SQL-driven hypothesis testing, and interactive Tableau dashboards, this project provides a complete analytical framework for understanding the relationship between pricing strategy, sales performance, profitability, and customer behaviour.

👤 Author

Vinay Kumar

Data Analytics | Business Analytics | SQL | Python | Tableau | Power BI
