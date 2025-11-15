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

