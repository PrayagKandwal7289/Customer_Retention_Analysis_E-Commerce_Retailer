# Customer Retention Analysis for a Canadian E-Commerce Retailer

## Project Overview

This project analyzes customer purchasing behavior for a Canadian e-commerce retailer using Python. The objective is to understand customer retention patterns, identify churned customers, and provide business recommendations to improve customer loyalty and long-term revenue growth.

The analysis was performed on transaction-level data containing customer information, product categories, locations, quantities purchased, and prices in Canadian dollars.

---

## Business Problem

Customer retention is critical for sustainable business growth. The company wants to:

* Identify customers at risk of churning.
* Understand purchasing behavior across provinces and product categories.
* Recognize high-value customers.
* Develop strategies to increase customer loyalty and repeat purchases.

For this project:

**Churned Customer = A customer who has not made a purchase in the last 90 days relative to the latest transaction date.**

---

## Objectives

* Clean and validate transactional data.
* Calculate key business KPIs.
* Segment customers into Active, At Risk, and Churned groups.
* Analyze revenue by province and product category.
* Identify top-performing customers.
* Generate actionable business recommendations.

---

## Tools & Technologies

* Python
* Pandas
* NumPy
* Matplotlib
* Google Colab

---

## Dataset Information

* Total transactions: 102,837
* Missing Customer IDs removed: 8,105
* Invalid quantity records removed: 4,810
* Final customers analyzed: 4,958

---

## Data Cleaning Steps

### Missing Customer IDs

8,105 transactions contained missing customer IDs. These records were removed because customer retention analysis requires unique customer identifiers.

### Duplicate Records

No duplicate rows were found in the dataset.

### Invalid Quantities

4,810 transactions contained zero or negative quantities. These records were removed because they likely represented returns, cancellations, or data-entry issues.

### Invalid Prices

No products contained invalid or negative prices.

### Feature Engineering

The following features were created:

* Revenue = Quantity × UnitPrice_CAD
* Month (derived from InvoiceDate)
* Days_Inactive
* Customer_Status

---

## Customer Segmentation Logic

| Customer Status | Definition                        |
| --------------- | --------------------------------- |
| Active          | Purchased within the last 30 days |
| At Risk         | No purchase for 31–90 days        |
| Churned         | No purchase for more than 90 days |

---

## Key Business Metrics

| Metric            | Value  |
| ----------------- | ------ |
| Total Customers   | 4,958  |
| Active Customers  | 1,751  |
| At-Risk Customers | 1,504  |
| Churned Customers | 1,703  |
| Churn Rate        | 34.35% |

---

## Top Provinces by Revenue

| Province | Revenue (CAD) |
| -------- | ------------: |
| ON       |     5,463,935 |
| BC       |     3,023,126 |
| QC       |     2,178,900 |
| AB       |     1,940,166 |
| SK       |       447,893 |

---

## Top Product Categories

| Category           | Revenue (CAD) |
| ------------------ | ------------: |
| Sports & Outdoors  |     3,134,334 |
| Clothing & Apparel |     2,782,049 |
| Home & Kitchen     |     2,508,020 |
| Electronics        |     2,377,082 |
| Baby & Kids        |     1,498,177 |

---

## Top Customers

| Customer ID | Revenue (CAD) | Orders |
| ----------- | ------------: | -----: |
| CUST03761   |        18,025 |     38 |
| CUST04098   |        17,656 |     40 |
| CUST03425   |        17,514 |     38 |
| CUST00621   |        17,339 |     38 |
| CUST03089   |        17,043 |     38 |

---

## Key Findings

### 1. Customer churn remains significant

Approximately 34% of customers have churned, highlighting opportunities for retention initiatives and re-engagement campaigns.

### 2. High-value customers drive substantial revenue

The highest-value customers generated over CAD 17,000 each and placed nearly 40 orders, demonstrating strong repeat purchasing behavior.

### 3. Ontario is the strongest market

Ontario generated more than CAD 5.4 million in revenue, making it the company's most important region.

### 4. Sports & Outdoors leads product performance

Sports & Outdoors was the highest-performing category, followed by Clothing & Apparel and Home & Kitchen.

### 5. A large at-risk segment exists

More than 1,500 customers are currently at risk of churning and should be targeted through proactive retention campaigns.

---

## Business Recommendations

### Launch Win-Back Campaigns

Target churned customers with personalized promotions and discount offers to encourage repeat purchases.

### Protect At-Risk Customers

Implement automated email campaigns for customers inactive for 31–90 days before they become fully churned.

### Strengthen Loyalty Programs

Reward high-value customers through VIP memberships, exclusive discounts, and early access to new products.

### Prioritize High-Revenue Provinces

Continue investing marketing resources in Ontario, British Columbia, and Quebec while exploring growth opportunities in smaller markets.

### Expand High-Performing Categories

Increase investment in Sports & Outdoors and Clothing & Apparel products to capitalize on strong customer demand.

---

## Skills Demonstrated

### Python

* Variables and functions
* Conditional logic
* Data manipulation workflows

### Pandas

* read_csv()
* groupby()
* agg()
* sort_values()
* value_counts()
* reset_index()
* isnull()
* dropna()
* to_datetime()

### NumPy

* np.where()

### Data Analysis

* Exploratory Data Analysis (EDA)
* Data Cleaning
* Feature Engineering
* Customer Segmentation
* Customer Retention Analysis
* Business KPI Development

### Data Visualization

* Bar Charts
* Line Charts
* Business Reporting

---

## Future Improvements

Potential enhancements include:

* RFM (Recency, Frequency, Monetary) Analysis
* Customer Lifetime Value Modeling
* Cohort Analysis
* Predictive Churn Modeling
* Interactive Power BI Dashboard

---

## Author

**Prayag Kandwal**

Aspiring Data Analyst | Python | SQL | Excel | Power BI

