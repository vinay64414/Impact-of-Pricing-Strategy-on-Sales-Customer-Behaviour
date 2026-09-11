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
