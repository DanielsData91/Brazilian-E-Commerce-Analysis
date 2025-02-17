# CareerFoundry-Project-Brazilian E-Commerce Analysis

![Brazilian E-Commerce](Visualizations/E-Commerce.jpg)

This project focuses on uncovering hidden sales patterns using Python through exploratory data analysis of demographic information. The sales behavior of different customer profiles was descriptively analyzed and compared using a heatmap.

This project focuses on uncovering hidden sales patterns using Python through exploratory data analysis in 
-1. __Revenue Analysis__
-2. __Customer Segmentation Analysis__
-3. __Efficiency Analysis__
-4. __Product Performance Analysis__
_5. __Time-based Trend Analysis__ .

The hypothesis testing was conducted by **Regression Analysis** and **Clustering Analysis**

__Hypothesis__ 

- Hypothesis 1: If shipping time is higher, then the shipping duration is higher?
- Hypothesis 2: If the price is higher, then the freight value is higher?
- Hypothesis 3: If the estimated duration is higher, then the freight value is higher?


## 1. Project Description
As a data analyst in this Project, I conducted an exploratory analysis of revenue, customer segmentation, shipping, and products. The objective was to analyze the current situation of the Brazilian E-Commerce Company to help develop a strategy for starting a franchise program. Key questions included identifying the best-performing products in terms of review score and shipping performance, analyzing the difference between actual shipping and estimated shipping time, and looking for strong correlations regarding the review scores. Moreover, exploring the sales performance across different states and identifying customers with a high lifetime value. The insides provided informed stakeholders developing the new franchise program for the company.


## 2.Documents
## 2.1 Project Management Folder
This folder contains the project brief, which explains the project guidelines and the data ERD.

## 2.2 Visualizations
This folder contains all necessary information about the visualizations to support the findings of the analysis.

## 2.3 __Brazilian E-Commerce__
This is the notebook, where you can find all the codes, output, and insights. Besides the maps for

**High Lifetime Customers per State**
![High_lifetime](file:///Users/daniel/Desktop/Ordner/Data%20Analyst/Data%20Analytics%20Course/Data%20Immersion/Achievement%206/Master%20Folder%20-%20Project%20Achievement%206%20update/Analysis/Maps/High_CLV_on_State_Level.html)

**Revenue Across the States**
![Revenue_States](file:///Users/daniel/Desktop/Ordner/Data%20Analyst/Data%20Analytics%20Course/Data%20Immersion/Achievement%206/Master%20Folder%20-%20Project%20Achievement%206%20update/Analysis/Maps/Total%20Revenue%20on%20State%20Level.html)

which would size up the script above 25MB which is not uploadable here in GitHub.

## 2.4 Data
#### 2.4.1 Original Data
The original data sets can be found on Kaggle.
![Original Data Set]([file:///Users/daniel/Desktop/Ordner/Data%20Analyst/Data%20Analytics%20Course/Data%20Immersion/Achievement%206/Master%20Folder%20-%20Project%20Achievement%206%20update/Analysis/Maps/Total%20Revenue%20on%20State%20Level.html](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce?select=olist_order_items_dataset.csv))

#### 2.4.2 Prepared Data

● The prepared data sets can be found on my Google Drive
![Prepared Data Set]([file:///Users/daniel/Desktop/Ordner/Data%20Analyst/Data%20Analytics%20Course/Data%20Immersion/Achievement%206/Master%20Folder%20-%20Project%20Achievement%206%20update/Analysis/Maps/Total%20Revenue%20on%20State%20Level.html](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce?select=olist_order_items_dataset.csv)](https://drive.google.com/drive/folders/16D2UfPa7iGCbDfkg-XrlKE_S2BxnVGXS?usp=drive_link))

## 2.5. __Business Questions__

__Revenue Analysis__
- 1: What is the average revenue per order, and how does is vary acroos different product categories?
- 2: Does revenue differ accross regions in Brazil?

__Customer Segmentation Analysis__
- 1: Where are customers with a high lifetime value located?
- 2: What is the customer satifsfaction level?
- 3: Do customers who leave a higher review show higher loyalty?

__Efficiency Analysis__
- 1: How close are the actual delivery time and estimated delivery time?
- 2: What is the impact of the freight value on the estimated delivery time?

__Product Performance__
- 1: What are the top 10 products in terms of total sales?
- 2: What are the top 10 products in terms of total quantity sales?
- 3: Which products have shortest shipping time on average?
- 4: What are the highest and lowest rated product categories?

__Time-based Trends__
- 1: Are there seasonal trends in sales volumne and revenue?
***


## 2.6. __Hypothesis__ 

- Hypothesis 1: If shipping time is higher, then the shipping duration is higher?
- Hypothesis 2: If the price is higher, then the freight value is higher?
- Hypothesis 3: If the estimated duration is higher, then the freight value is higher?


## 3.__Insights to the Key Questions
#### 3.1__Revenue Analysis__
- 1: What is the average revenue per order, and how does it vary acroos different product categories?

![Avg. Rev. per Order by Product Category](https://github.com/DanielsData91/Brazilian-E-Commerce-Analysis/blob/main/Visualizations/rev_prod_cat.png))

Insights:
product_category_name_english
security_and_services                162.255000
furniture_mattress_and_upholstery    158.385714
office_furniture                     145.815604
home_appliances_2                    141.910533
la_cuisine                           134.713333
furniture_bedroom                    133.022222
watches_gifts                        132.089943
air_conditioning                     131.988526
cool_stuff                           131.757731
home_confort                         127.486860
Name: total_rev_order, dtype: float64

- 2: Does revenue differ accross regions in Brazils

![Rev. Across States](https://github.com/DanielsData91/Brazilian-E-Commerce-Analysis/blob/main/Visualizations/Total%20Revenue%20States.png)

Insight: The highest revenue across Brazil is accounted for

São Paulo - with a total revenue of 3534861.50
Rio de Janeiro - with a total revenue of 1127145.03
Minas Gerais - with a total revenue of 1039629.78



#### 5.2_Customer Segmentation Analysis__
- 1: Where are customers with a high lifetime value located?
 ![High Lifetime Customers](https://github.com/DanielsData91/Brazilian-E-Commerce-Analysis/blob/main/Visualizations/Hihg%20Lifetime%20Customers.png)

Insights: The customers with the highest lifetime value are based in

praia grande
niteroi
belo horizonte

- 
- 2: What is the customer satisfaction level?
 ![Customer Satisfaction Level ](https://github.com/DanielsData91/Brazilian-E-Commerce-Analysis/blob/main/Visualizations/satisfaction_level.png)

Insights: Review scores of 4 and 5 are given the most by all customers, which leads to satisfaction level of 76.57%


- 3: Do customers who leave a higher review show higher loyalty?

 ![Loyalty_Review](https://github.com/DanielsData91/Brazilian-E-Commerce-Analysis/blob/main/Visualizations/loyalty_review.png)

__Insights:__ It seems that customers which are giving an higher review score are also the most loyal. That can be oberserved by the increasing number of orders for each review score level.

#### 5.3 __Efficiency Analysis__
- 1: How close are the actual delivery time and estimated delivery time?
 ![Difference_Time](https://github.com/DanielsData91/Brazilian-E-Commerce-Analysis/blob/main/Visualizations/diff_delivery.png)

   on_time  count  percentage
0        1  80073   93.566179
1        0   5506    6.433821

__Insights:__ 93% of all orders are on time. The most of those orders are even delivered before the estimated delivery date. Looking at the bar graph shows that the date of delivery is 10 to 20 days earlier than expected.
  
- 2: What is the impact of the freight value on the estimated delivery time?
![Time_Freight](https://github.com/DanielsData91/Brazilian-E-Commerce-Analysis/blob/main/Visualizations/freight_vs_shiptime.png)

Insights
__Insights:__ According to the scatterplot and previous created heatmap show no relationship between freight value and shipping time. That means that early shippings as well as delayed shipping are not impacted by the freight value of the items.

#### 5.4 __Product Performance__
- 1: What are the top 10 products in terms of total sales?

- ![Top 10](https://github.com/DanielsData91/Brazilian-E-Commerce-Analysis/blob/main/Visualizations/top10_prod.png)

__Insights:__ The top ten products are 
1. 99a4788cb24856965c36a24e339b6058  **bed_bath_table** with a revenue of **47190.28**
2. 3dd2a17168ec895c781a9191c1e95ad7  **computers_accessories** with a revenue of **34575.24**
3. e0d64dcfaa3b6db5c54ca298ae101d05  **watches_gifts** with a revenue of **33724.13**
4. aca2eb7d00ea1a7b8ebd4e68314663af  **furniture_decor** with a revenue of **30438.97**
5. f1c7f353075ce59d8a6f3cf58f419c9c  **bed_bath_table** with a revenue of **28155.01**
6. 2b4609f8948be18874494203496bc318  **health_beauty** with a revenue of **26174.20**
7. 5a848e4ab52fd5445cdc07aab1c40e48  **bed_bath_table** with a revenue of **25474.59**
8. 7a10781637204d8d10485c71a6108a2e  **watches_gifts** with a revenue of **24757.06**
9. 422879e10f46682990de24d770e7f83d  **garden_tools** with a revenue of **22022.39**
10. 389d119b48cf3043d311335e499d9c6b  **garden_tools** with a revenue of **20505.44**
  
- 2: What are the top 10 products in terms of total quantity sales?
- ![Top 10_qty](https://github.com/DanielsData91/Brazilian-E-Commerce-Analysis/blob/main/Visualizations/top10_prod_qty.png)

- __Insights:__ Top 3 categories
1. The product category of **bed_bath_table** sold **11810** items in total
2. The product category of **health_beauty** sold **8084** items in total
3. The product category of **sports_leisure** sold **7594** items in total
- 
- 3: Which products have shortest shipping time on average?

product_category_name_english	
security_and_services	-17.000000
la_cuisine	-16.777778
furniture_bedroom	-16.000000
cds_dvds_musicals	-15.818182
fixed_telephony	-15.494565
...	...
food	-9.768879
home_confort	-9.732558
home_comfort_2	-8.708333
arts_and_craftmanship	-6.227273
computers	-2.000000

__Insights:__ The fastes shipping time on average are accounted in the category of security and services, la cuisine and furniture bedroom.


- 4: What are the highest and lowest rated product categories?
- ![high_score](https://github.com/DanielsData91/Brazilian-E-Commerce-Analysis/blob/main/Visualizations/high_score_cat.png)

- - ![low_score](https://github.com/DanielsData91/Brazilian-E-Commerce-Analysis/blob/main/Visualizations/low_score_cat.png)

__Insights:__ The top 10 categories score on average a review above 4. Whereas the categories with the lowest score from 2 to closely 4. That means that all products (high & low) are receiving on average an **good - very good score**.


#### 5.5 __Time-based Trends__
- 1: Are there seasonal trends in sales volumne and revenue?

- - ![sales_rev](https://github.com/DanielsData91/Brazilian-E-Commerce-Analysis/blob/main/Visualizations/season_sales_rev.png)
 
![sales_qty](https://github.com/DanielsData91/Brazilian-E-Commerce-Analysis/blob/main/Visualizations/season_sales_vol.png)

__Insights:__ There is no clear seasonal pattern visible, beside that the sales drop around **June** and **July** and increase in **August**.

## 6.Hypothesis


- Hypothesis 1: If shipping time is higher, then the shipping duration is higher?
- 
![timevsduration](https://github.com/DanielsData91/Brazilian-E-Commerce-Analysis/blob/main/Visualizations/timevsduration.png)

__Interpretation on the fit of the regression model__: The first thing to notice is that the line covers a small amount of data points since most data points are gathered on a higher y-axis value as well as the huge cluster of points around the shipping time -50 - +50 days and shipping duration 0-50 days, the line shows a strong positive regression, which will be explored further later on.

Summary Statistics

	Actual	Predicted
0	6.0	10.707795
1	12.0	17.827561
2	14.0	10.160121
3	2.0	8.517098
4	45.0	32.067091
5	17.0	13.446167
6	12.0	15.089189
7	2.0	11.255470
8	4.0	12.898492
9	17.0	16.732212
10	10.0	8.517098
11	11.0	13.993841
12	7.0	9.064773
13	16.0	9.612447
14	24.0	9.612447
15	9.0	10.160121
16	12.0	15.089189
17	3.0	16.184538
18	11.0	-2.436387
19	10.0	9.064773


__Thought:__

- There is a positive relationship between shipping time and shipping duration, but the relationship is weak (R² = 0.38).
- MSE is quite high, meaning predictions deviate significantly from actual durations.
- Linear regression is not capturing the complexity of the data well, and the presence of negative predictions is a warning sign.
- Further investigation into other features (e.g., distance, product type, region) or trying a different model (e.g., decision trees, random forest) could improve predictive power.
- 
- Hypothesis 2: If the price is higher, then the freight value is higher?


- ![pricevsfreight](https://github.com/DanielsData91/Brazilian-E-Commerce-Analysis/blob/main/Visualizations/pricevsfreight.png)

__Interpretation on the fit of the regression model__: The line covers only points in the middle of the scatter plot. Reaching from freight value 13 to price 250. The line shows a positive regression.

Summary Statistics
	Actual	Predicted
0	27.30	16.034774
1	13.18	15.997385
2	16.73	15.470183
3	7.78	13.943717
4	16.37	19.800504
5	15.89	17.998602
6	12.32	15.966990
7	13.21	16.581611
8	8.23	17.377257
9	19.50	16.032353
10	15.42	14.824629
11	15.23	14.687449
12	18.65	15.712266
13	10.96	14.283978
14	24.72	15.897862
15	11.74	14.313566
16	13.37	14.956430
17	9.41	15.470183
18	20.83	15.090920
19	13.24	17.353048



__Thought:__

- Low predictive power: The R² score is quite low, indicating that "Price" alone is not a strong predictor of "Freight Value". There may be other important variables not included in the model.

- Potential improvements: You might want to include other variables, such as product category, shipping distance, or order size, to improve the model's accuracy. Alternatively, exploring more complex models could help capture any non-linear relationships.


- Hypothesis 3: If the estimated duration is higher, then the freight value is higher?

- ![estivsfreight](https://github.com/DanielsData91/Brazilian-E-Commerce-Analysis/blob/main/Visualizations/estivsduration.png)

- __Interpretation on the fit of the regression model__: The line covers many points of the cluster. But looking at the statistic summary will show a better picture for interpretation.

- Summary Statistics
	Actual	Predicted
0	27.30	14.769862
1	13.18	12.863420
2	16.73	17.221002
3	7.78	14.769862
4	16.37	14.769862
5	15.89	16.403955
6	12.32	14.225164
7	13.21	13.408117
8	8.23	13.135769
9	19.50	14.769862
10	15.42	16.948653
11	15.23	14.497513
12	18.65	15.859257
13	10.96	18.038048
14	24.72	20.216839
15	11.74	15.859257
16	13.37	14.225164
17	9.41	11.229326
18	20.83	22.667979
19	13.24	16.676304
__Thought:__

- Modest predictive power: The R² score of 0.208 is still low, suggesting that Estimated Duration Days has a weak relationship with Freight Value on its own. The model might benefit from incorporating additional variables to improve its accuracy.

## 7. Recommendations
## 8.Next Steps


