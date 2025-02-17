# CareerFoundry Project: Brazilian E-Commerce Analysis

![Brazil](https://github.com/DanielsData91/Brazilian-E-Commerce-Analysis/blob/main/Visualizations/E-Commerce.jpg)

## Overview
This project aims to uncover hidden sales patterns through exploratory data analysis using Python. The analysis focuses on customer demographics, purchasing behavior, and operational efficiency. Various analytical techniques, including regression and clustering analysis, were applied to gain insights into revenue, customer segmentation, shipping performance, product performance, and time-based sales trends.

## Key Analytical Areas
- **Revenue Analysis**
- **Customer Segmentation Analysis**
- **Efficiency Analysis**
- **Product Performance Analysis**
- **Time-based Trend Analysis**

## Hypothesis Testing
Hypotheses were tested using Regression Analysis and Clustering Analysis:

- **Hypothesis 1:** Higher shipping time leads to longer shipping durations.
- **Hypothesis 2:** Higher product prices correlate with higher freight values.
- **Hypothesis 3:** Longer estimated shipping durations result in higher freight values.

---

## 1. Project Description
As a data analyst for this project, I conducted an exploratory analysis focusing on revenue, customer segmentation, shipping efficiency, and product performance. The goal was to assess the current state of a Brazilian e-commerce company and support the development of a franchise program. Key objectives included identifying top-performing products, assessing shipping efficiency, and locating high-value customers.

---

## 2. Project Documentation
### 2.1 Project Management Folder
Contains the project brief outlining guidelines and an entity-relationship diagram (ERD) of the data.

### 2.2 Visualizations
Contains visualizations supporting the findings from the analysis.

### 2.3 Brazilian E-Commerce Notebook
This Jupyter Notebook contains the code, outputs, and insights. Interactive maps illustrating:
- High Lifetime Value Customers by State
- Revenue Distribution Across States

**Note:** Due to file size limitations, these maps exceed 25MB and are not uploaded to GitHub.

### 2.4 Data
#### 2.4.1 Original Data
Available on Kaggle: [Brazilian E-Commerce Public Dataset](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

#### 2.4.2 Prepared Data
Available on Google Drive: [Prepared Dataset](https://drive.google.com/drive/folders/YOUR_LINK_HERE)

### 2.5 Business Questions
#### Revenue Analysis
- What is the average revenue per order, and how does it vary across product categories?
- How does revenue distribution vary across Brazilian states?

#### Customer Segmentation Analysis
- Where are high lifetime value customers located?
- What is the overall customer satisfaction level?
- Do higher review scores indicate higher customer loyalty?

#### Efficiency Analysis
- How accurate are estimated delivery times compared to actual delivery times?
- Does freight value impact estimated delivery times?

#### Product Performance Analysis
- What are the top 10 products by total sales revenue?
- What are the top 10 products by total quantity sold?
- Which product categories have the shortest average shipping times?
- Which product categories receive the highest and lowest review scores?

#### Time-based Trend Analysis
- Are there any seasonal trends in sales volume and revenue?

---

## 3. Key Insights and Findings
### 3.1 Revenue Analysis
- **Average Revenue per Order:** Security and Services, Furniture, and Home Appliances categories generate the highest average revenue per order.

![Avg_Rev](https://github.com/DanielsData91/Brazilian-E-Commerce-Analysis/blob/main/Visualizations/rev_prod_cat.png)

- **Regional Revenue Distribution:** The top states by revenue are São Paulo (R$3,534,861.50), Rio de Janeiro (R$1,127,145.03), and Minas Gerais (R$1,039,629.78).

![Total_Rev_States](https://github.com/DanielsData91/Brazilian-E-Commerce-Analysis/blob/main/Visualizations/Total%20Revenue%20States.png)

### 3.2 Customer Segmentation Analysis
- **High Lifetime Value Customers:** Concentrated in Praia Grande, Niterói, and Belo Horizonte.

![High_LT_Cust](https://github.com/DanielsData91/Brazilian-E-Commerce-Analysis/blob/main/Visualizations/Hihg%20Lifetime%20Customers.png)
  
- **Customer Satisfaction:** 76.57% of reviews are positive (scores 4 or 5).

![Sat_Level](https://github.com/DanielsData91/Brazilian-E-Commerce-Analysis/blob/main/Visualizations/satisfaction_level.png)

- **Loyalty and Review Scores:** Higher review scores correlate with increased order frequency, indicating loyal customers tend to leave positive reviews.

![Loyalty](https://github.com/DanielsData91/Brazilian-E-Commerce-Analysis/blob/main/Visualizations/loyalty_review.png)

### 3.3 Efficiency Analysis
- **Delivery Time Accuracy:** 93.57% of orders are delivered on or before the estimated delivery date, with many arriving 10-20 days early.

![Diff_Shipping](https://github.com/DanielsData91/Brazilian-E-Commerce-Analysis/blob/main/Visualizations/diff_delivery.png)

- **Freight Value vs. Delivery Time:** No clear relationship between freight value and delivery time.

![FreightVSShipping_Time](https://github.com/DanielsData91/Brazilian-E-Commerce-Analysis/blob/main/Visualizations/freight_vs_shiptime.png)


### 3.4 Product Performance Analysis
- **Top Products by Revenue:** Notable products are from categories like Bed Bath Table, Computers Accessories, and Watches Gifts.

![Top10_Prods](https://github.com/DanielsData91/Brazilian-E-Commerce-Analysis/blob/main/Visualizations/top10_prod.png)
  
- **Top Products by Quantity:** Bed Bath Table, Health Beauty, and Sports Leisure lead in sales volume.

![Top10_QTY](https://github.com/DanielsData91/Brazilian-E-Commerce-Analysis/blob/main/Visualizations/top10_prod_qty.png)
  
- **Fastest Shipping Categories:** Security and Services, La Cuisine, and Furniture Bedroom products have the shortest average shipping times.
  
![Fastest](https://github.com/DanielsData91/Brazilian-E-Commerce-Analysis/blob/main/Visualizations/Fastest_Delivery.png)


- **Product Ratings:** High-rated categories average above 4 stars, while lower-rated categories still average near 4 stars, indicating generally positive reviews across products.

![Top_score](https://github.com/DanielsData91/Brazilian-E-Commerce-Analysis/blob/main/Visualizations/high_score_cat.png)

![Bottom_Score](https://github.com/DanielsData91/Brazilian-E-Commerce-Analysis/blob/main/Visualizations/low_score_cat.png)

### 3.5 Time-based Trends
- **Seasonal Sales Trends:** No strong seasonal pattern detected. However, sales dip in June and July, with a recovery in August.

![Sales_Rev](https://github.com/DanielsData91/Brazilian-E-Commerce-Analysis/blob/main/Visualizations/season_sales_rev.png)

![Sales_Vol](https://github.com/DanielsData91/Brazilian-E-Commerce-Analysis/blob/main/Visualizations/season_sales_vol.png)

---
## 4. Hypothesis

- **Hypothesis 1:** If shipping time is higher, then the shipping duration is higher?

![TimeVSDuration](https://github.com/DanielsData91/Brazilian-E-Commerce-Analysis/blob/main/Visualizations/timevsduration.png)

**Interpretation of the Regression Model Fit:**

The first observation is that the regression line covers a relatively small number of data points, as most of the points are concentrated around higher y-axis values. Additionally, there is a large cluster of points around a shipping time of -50 to +50 days and a shipping duration of 0-50 days. Despite this concentration, the regression line shows a strong positive correlation, which will be further explored later.

![TimeVSDuration](https://github.com/DanielsData91/Brazilian-E-Commerce-Analysis/blob/main/Visualizations/Hypothesis%201.png)

**Thought:**

- There is a positive relationship between shipping time and shipping duration, though the relationship is weak (R² = 0.38).
- The Mean Squared Error (MSE) is quite high, indicating that predictions deviate significantly from actual values.
- The linear regression model does not capture the complexity of the data well, and the presence of negative predictions is a red flag.
- Further investigation into other features (e.g., distance, product type, region) or experimenting with different models (e.g., decision trees, random forests) could improve predictive power.

---

- **Hypothesis 2:** If the price is higher, then the freight value is higher?
  
![PrceVSFreight](https://github.com/DanielsData91/Brazilian-E-Commerce-Analysis/blob/main/Visualizations/pricevsfreight.png)

**Interpretation of the Regression Model Fit:**

The regression line covers only the middle range of the scatter plot, spanning freight values from 13 to prices around 250. The line suggests a positive correlation between price and freight value.

![Hypothesis 2](https://github.com/DanielsData91/Brazilian-E-Commerce-Analysis/blob/main/Visualizations/Hypothesis%202.png)

**Thought:**
- Low predictive power: The R² score is low, indicating that "Price" alone is not a strong predictor of "Freight Value." Other important variables may be missing from the model.
- Potential improvements: Including additional variables, such as product category, shipping distance, or order size, could improve the model’s accuracy. Alternatively, exploring more complex models might help capture any non-linear relationships.

---

- **Hypothesis 3:** If the estimated duration is higher, then the freight value is higher??

![EstiDurationVSFreight](https://github.com/DanielsData91/Brazilian-E-Commerce-Analysis/blob/main/Visualizations/estivsduration.png)

**Interpretation of the Regression Model Fit:**

The regression line fits many of the data points in the cluster, but a more detailed statistical summary will provide a clearer interpretation.

![Hypothesis 3](https://github.com/DanielsData91/Brazilian-E-Commerce-Analysis/blob/main/Visualizations/Hypothesis%203.png)

**Thought:**
- Modest predictive power: The R² score of 0.208 suggests a weak relationship between the Estimated Duration Days and Freight Value.
- The model might benefit from incorporating additional variables to enhance its accuracy

---

## 5. Recommendations
Based on the findings, the following actions are recommended:

- **Focus on High-Value States:** Prioritize expanding in São Paulo, Rio de Janeiro, and Minas Gerais due to high revenue potential.
- **Leverage High Lifetime Value Customers:** Engage top customers in Praia Grande, Niterói, and Belo Horizonte with loyalty programs and targeted offers.
- **Optimize Top-Selling Categories:** Strengthen product offerings in Bed Bath Table, Computers Accessories, and Health Beauty categories.
- **Improve Delivery Communication:** Capitalize on early deliveries by promoting reliable and fast delivery as a competitive advantage.
- **Maintain Customer Satisfaction:** Continue focusing on product quality and service to maintain positive reviews and strengthen customer loyalty.
- **Explore Seasonal Promotions:** Investigate causes of sales dips in June-July and develop promotional campaigns to counteract this trend.

---

## 6. Next Steps
- **Detailed Market Analysis:** Conduct a deeper regional analysis focusing on customer preferences and local competition.
- **Customer Retention Strategies:** Implement targeted marketing campaigns and loyalty programs for high-value customers.
- **Operational Efficiency:** Investigate logistics partners and processes to maintain or improve early delivery performance.
- **Product Expansion:** Evaluate potential for expanding high-performing categories into underpenetrated regions.
- **Seasonality Research:** Further investigate the June-July sales dip to determine underlying causes and refine promotional strategies accordingly.

---

## Contact
For further information or questions about this project, feel free to connect with me on [LinkedIn](https://www.linkedin.com/in/daniel-m%C3%BCller-profile) or check out my other projects on [GitHub](https://github.com/DanielsData91).






