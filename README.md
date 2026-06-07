# Customer Segmentation Using K-Means Clustering

## Project Overview

This project focuses on segmenting customers based on their purchasing behavior using K-Means Clustering, an unsupervised machine learning algorithm. The objective is to identify meaningful customer groups that can help businesses develop targeted marketing, retention, and profitability strategies.

Customer-level features were created from transactional data, including sales, profit, order frequency, and recency. These features were used to discover distinct customer segments and generate actionable business insights.

---

## Business Problem

Businesses often serve customers with different purchasing behaviors and value levels. Treating all customers the same can lead to inefficient marketing efforts and missed opportunities.

The goal of this project is to:

* Identify distinct customer groups based on purchasing behavior.
* Understand the characteristics of each customer segment.
* Generate business recommendations for marketing and retention strategies.

---

## Dataset Information

### Dataset

Sample Superstore Dataset

### Dataset Size

* Rows: 9,994
* Columns: 21

### Key Features

* Customer ID
* Customer Name
* Sales
* Profit
* Quantity
* Order Date

---

## Feature Engineering

Since clustering should be performed at the customer level, transactional records were aggregated to create customer-level metrics:

### Customer Features

* Total Sale
* Total Profit
* Total Orders
* Recency

### Recency

Recency represents the number of days since a customer's last purchase.

* Lower Recency → More Active Customer
* Higher Recency → Less Active Customer

---

## Project Workflow

1. Data Understanding
2. Data Cleaning
3. Customer-Level Aggregation
4. Feature Engineering
5. Feature Scaling
6. Elbow Method
7. Silhouette Score Analysis
8. K-Means Clustering
9. Cluster Analysis
10. Business Insights

---

## Clustering Approach

### Feature Scaling

StandardScaler was applied to ensure all features contributed equally during distance calculations.

### Elbow Method

The Elbow Method suggested an optimal cluster count of **4**.

### Silhouette Score

Silhouette Score analysis confirmed that **4 clusters** provided the best balance between cluster cohesion and separation.

---

## Customer Segments Identified

### Cluster 0 – Unprofitable High-Value Customers

Characteristics:

* High sales
* Negative profit
* Moderate order frequency
* Recent activity

Business Action:

* Review discount policies
* Improve profit margins
* Analyze shipping and operational costs

---

### Cluster 1 – Regular Customers

Characteristics:

* Moderate sales
* Moderate profit
* Consistent purchasing behavior

Business Action:

* Upselling opportunities
* Cross-selling campaigns
* Loyalty incentives

---

### Cluster 2 – Inactive Customers

Characteristics:

* Low sales
* Low order frequency
* Very high recency

Business Action:

* Re-engagement campaigns
* Promotional offers
* Personalized marketing

---

### Cluster 3 – Loyal High-Value Customers

Characteristics:

* High sales
* High profit
* Highest order frequency

Business Action:

* VIP programs
* Exclusive offers
* Customer retention initiatives

---

## Key Insights

* Four meaningful customer segments were identified using K-Means Clustering.
* Regular Customers represent the majority of the customer base.
* Loyal High-Value Customers contribute significantly to revenue and profitability.
* Inactive Customers present opportunities for re-engagement and retention campaigns.
* Unprofitable High-Value Customers generate substantial sales but negatively impact profitability.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

---

## Future Improvements

* Apply PCA for cluster visualization.
* Experiment with Hierarchical Clustering and DBSCAN.
* Build an interactive customer segmentation dashboard using Power BI.
* Deploy customer segmentation insights through a web application.

---

## Conclusion

This project successfully applied K-Means Clustering to identify distinct customer segments based on purchasing behavior. The segmentation revealed valuable insights into customer value, engagement, and profitability. These findings can help businesses design targeted marketing campaigns, improve customer retention, and make data-driven strategic decisions.
