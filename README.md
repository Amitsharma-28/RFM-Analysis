# RFM Analysis — Custom Printing Business

## Project Background
PrintPlus Studios, established in 2019, is a growing e-commerce company specialising in personalised print products such as canvas artwork, posters, flyers, and business cards. Operating entirely online, the company serves customers through its website, offering fast turnaround times and fully customisable design options.

The business generates substantial amounts of data from its daily transactions, customer interactions, and product sales. However, much of this information has been historically underutilised. This project leverages Excel-based analysis to transform raw order data into meaningful insights using an RFM (Recency, Frequency, Monetary) framework. By doing so, it uncovers key customer segments and provides actionable recommendations aimed at improving customer retention, marketing effectiveness, and long-term commercial performance.

The goal is to answer three key business questions:

**1. Who are the best customers?**  

**2. Who needs a retention campaign?**  

**3. Which segments are safe to ignore?**

All the Excel formulas used for the analysis can be found [here](https://github.com/user-attachments/files/23559866/Formulas_RFMAnalysis.docx).

## Data Overview & Initial Checks
PrintPlus Studios transaction-level dataset contains one year of customer order history with a total row count of 1000 records.

The dataset includes the following fields:

- **OrderID:** Identifies each individual transaction uniquely.

- **CustomerID:** Indicates which customer placed the order.

- **OrderDate:** Indicates the date the purchase was made.

- **ProductType:** Indicates the type of printed product purchased.

- **OrderValue:** Specifies the total monetary amount of the order, measured in Indian Rupees (₹).

The image below displays a snippet of the dataset.
<p align="center"><img width="577" height="471" alt="data fields " src="https://github.com/user-attachments/assets/9fa75124-9a3f-4f63-bbeb-f34c00a3a172" />
</p>

Prior to beginning the analysis, a variety of checks were conducted for quality control and familiarization with the dataset. These included identifying duplicate OrderID values, checking for blanks in critical fields (OrderDate, OrderValue, CustomerID), and verifying the earliest and latest transaction dates to confirm the accuracy of the analysis window.

## Executive Summary
**Overview of Findings**

The RFM analysis highlights three critical patterns in customer behaviour. First, the business has a strong and reliable core of 61 Best Customers, who consistently purchase at high frequency and generate substantial revenue. Second, 57 customers fall into the Need Attention group, indicating a sizeable portion of the customer base that once engaged well but has since become inactive—representing a clear opportunity for retention-focused campaigns. Finally, only 13 customers qualify as At Risk, showing very low commercial impact and limited potential for reactivation, suggesting that targeted marketing spend should not be directed toward this group.

These findings collectively show that while the business benefits from a healthy high-value cohort, it also faces a meaningful risk of losing mid-value customers who could be recovered with timely intervention. The segmentation therefore provides a clear roadmap for prioritising loyalty, reactivation, and cost-efficient marketing efforts.

**Best Customers**

- There are 61 best customers having an RFM score ≥ 13 out of 15, meaning their combined recency, frequency, and monetary value places them among the highest-value customers.

<p align="center"><img width="770" height="897" alt="Screenshot 2025-11-18 at 3 36 23 PM" src="https://github.com/user-attachments/assets/b956d2f7-3de8-4617-a677-10e6e388237d" /></p>

- 46% (28 customers) in this segment made purchases more recently than 80% of the entire customer base. 38% (23 customers) purchased more recently than 60% of customers, and 16% (10 customers) purchased more recently than 40% of customers. The Best Customer segment is composed largely of highly recent purchasers.
  
- 89% (54 customers) in this segment made purchases more frequently than 80% of the customer base, while the remaining 11% (7 customers) purchased more frequently than 60% of customers. The entire best customer segment consistently falls within the highest-frequency tiers, demonstrating strong loyalty and repeat buying behaviour.

- 74% (45 customers) in this segment spend more than 80% of all customers, 25% (15 customers) spend more than 60% of customers, and 5% (1 customer) spend more than 40% of customers. The best customer segment is largely composed of high-value spenders who  who generate a significant share of overall revenue.

**Need Attention**

- There are 57 Need Attention customers with an RFM score between 4 and 6 out of 15, indicating that their combined recency, frequency, and monetary performance places them in a low-engagement tier.

<p align="center"><img width="713" height="822" alt="Screenshot 2025-11-18 at 3 44 33 PM" src="https://github.com/user-attachments/assets/1382b4dd-6835-4fda-a65c-de20b37db224" /></p>

- 5% (3 customers) in this segment purchased more recently than 60% of the customer base, 16% (9 customers) purchased more recently than 40% of customers, 37% (21 customers) purchased more recently than 20% of customers, and 43% (24 customers) purchased less recently than 80% of customers, placing them in the bottom 20% for recency. The Need Attention segment is characterised by a substantial share of customers whose last purchase occurred a significant time ago, indicating declining engagement and an elevated risk of churn.

- 4% (2 customers) purchase more frequently than 40% of the customer base, 70% (40 customers) purchase more frequently than 20% of customers, and 26% (15 customers)  purchase less frequently than 80% of customers, placing them in the bottom 20% for purchase frequency. The need attention segment is dominated by customers with low purchase frequency, indicating limited repeat-buying behaviour and weaker purchasing consistency.

- 7% (4 customers) in this segment spend more than 40% of the customer base, 32% (18 customers) spend more than 20% of customers, and 61% (35 customers) spend less than 80% of customers, placing them in the bottom 20% for total spending. The Need Attention segment is predominantly composed of low-spending customers with limited revenue contribution.

**At Risk**

- There are 13 At Risk customers with an RFM score of 3 out of 15, indicating that their combined recency, frequency, and monetary performance places them in the lowest engagement tier, characterised by very infrequent purchases, long periods of inactivity, and minimal spending.

<p align="center"><img width="1052" height="333" alt="Screenshot 2025-11-18 at 3 48 48 PM" src="https://github.com/user-attachments/assets/7f9d04c3-5aa7-45d6-92d0-63affa9fb36c" /></p>

- 100% (13 customers) in this segment purchased less recently than 80% of the customer base, placing all of them in the bottom 20% for recency. The at risk segment has been inactive for a long period and shows a high likelihood of disengagement.

- 100% (13 customers) in this segment purchase less frequently than 80% of the customer base, placing them in the bottom 20% for purchase frequency. The at risk segment reflects consistently low repeat-buying behaviour, signalling weak loyalty and limited interaction with the business.

- 100% (13 customers) in this segment spend less than 80% of the customer base, placing them in the bottom 20% for total spending. The at risk segment contributes the lowest revenue levels in the dataset.

## Recommendations
