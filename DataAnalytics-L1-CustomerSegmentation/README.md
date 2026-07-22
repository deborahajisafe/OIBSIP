# Customer Segmentation Analysis using RFM and K-Means Clustering

## Project Overview
The objective of this project is to segment an e-commerce company's customers into distinct groups based on their purchasing behaviour using **RFM (Recency, Frequency, Monetary) Analysis** and the **K-Means Clustering Algorithm**.

Customer segmentation enables businesses to understand different customer groups and develop targeted marketing strategies to improve customer retention, increase sales, and maximize customer lifetime value.

## Objectives

- Perform data cleaning and preprocessing.
- Calculate customer purchasing behaviour using RFM Analysis.
- Standardize customer features using StandardScaler.
- Apply K-Means Clustering to segment customers.
- Determine the optimal number of clusters using the Elbow Method.
- Visualize customer segments.
- Provide business insights and marketing recommendations.

## Dataset

**Dataset:** Online Retail Dataset

The dataset contains transactional data from a UK-based online retail store.

It includes:

- Invoice Number
- Product Description
- Quantity Purchased
- Invoice Date
- Unit Price
- Customer ID
- Country

## Tools

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Project Workflow

### 1. Data Inspection

- Loaded the dataset
- Checked data types
- Examined missing values
- Identified duplicate records

### 2. Data Cleaning

- Removed records with missing Customer IDs
- Removed rows with missing product descriptions
- Removed cancelled transactions
- Removed transactions with negative quantity
- Removed transactions with negative unit prices

### 3. Feature Engineering

Created a new feature:

- **TotalAmount = Quantity × UnitPrice**

### 4. RFM Analysis

Calculated three customer behaviour metrics:

- **Recency** – Number of days since the customer's last purchase
- **Frequency** – Number of unique purchases made
- **Monetary** – Total amount spent by each customer

### 5. Data Standardization

Applied **StandardScaler** to ensure all RFM features contributed equally during clustering.

### 6. Customer Segmentation

Applied **K-Means Clustering**.

Used the **Elbow Method** to determine the optimal number of clusters.

**Optimal Number of Clusters (K): 4**

### 7. Data Visualization

Created:

- Elbow Method Plot
- Number of Customers per Cluster
- Frequency vs Monetary Scatter Plot
- Recency vs Monetary Scatter Plot

## Key Findings

The analysis identified four customer segments:

### Cluster 0 – Regular Customers

- Moderate purchase frequency
- Moderate spending
- Opportunity for increased engagement

### Cluster 1 – Inactive / At-Risk Customers

- Long time since last purchase
- Low spending
- Require re-engagement campaigns

### Cluster 2 – VIP Customers

- Highest purchase frequency
- Highest spending
- Most valuable customer segment

### Cluster 3 – Loyal Customers

- Frequent purchases
- High spending
- Strong candidates for loyalty rewards

## Business Recommendations

- Reward VIP customers with exclusive offers and premium services.
- Implement personalized marketing campaigns for loyal customers.
- Launch re-engagement campaigns for inactive customers.
- Encourage regular customers to purchase more frequently through loyalty programs and targeted promotions.