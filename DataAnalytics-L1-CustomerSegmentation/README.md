# Customer Segmentation Using K-Means Clustering

## 1. Project Overview

Customer segmentation is the process of dividing customers into distinct groups based on shared characteristics and behaviors. This project applies the **K-Means Clustering** algorithm to segment customers based on demographic and spending-related attributes.

The analysis aims to identify meaningful customer groups that can help businesses understand customer behavior and develop more targeted marketing strategies.

## 2. Objectives

The main objectives of this project are:

* To analyze customer demographic and spending data.
* To perform exploratory data analysis on customer attributes.
* To identify patterns and relationships within the dataset.
* To determine an appropriate number of customer segments using the Elbow Method.
* To apply K-Means Clustering for customer segmentation.
* To analyze and interpret the characteristics of the resulting clusters.
* To visualize the identified customer segments.

## 3. Dataset

The dataset contains information about customers and includes the following attributes:

 Feature                | Description                                              
 Customer ID             : Unique identifier assigned to each customer             
 Gender                  : Gender of the customer                                    
 Age                     : Age of the customer                                       
 Annual Income (k$)      : Annual income of the customer in thousands of dollars     
 Spending Score (1-100)  : Score assigned to the customer based on spending behavior 

The dataset used in this project is stored in:

`store_customers.csv`

## 4. Technologies and Libraries Used

The project was implemented using the following technologies:

* Python
* Jupyter Notebook
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

## 5. Methodology

### 5.1 Data Loading

The customer dataset was loaded using the Pandas library. The structure, dimensions, column names, data types, and basic statistical information were examined.

### 5.2 Exploratory Data Analysis

Exploratory data analysis was performed to understand the distribution of important customer attributes.

The following visualizations were created:

* Gender distribution
* Age distribution
* Annual income distribution
* Spending score distribution

### 5.3 Feature Selection

Relevant numerical features were selected for clustering, particularly customer income and spending behavior.

### 5.4 Determining the Optimal Number of Clusters

The **Elbow Method** was used to determine a suitable number of clusters for the K-Means algorithm. The Within-Cluster Sum of Squares (WCSS) was evaluated for different values of K.

### 5.5 K-Means Clustering

The K-Means Clustering algorithm was applied to the selected customer features. Each customer was assigned to one of the identified clusters based on similarity.

### 5.6 Cluster Analysis

The resulting clusters were analyzed using cluster summaries and cluster-size comparisons. The characteristics of each group were examined based on income and spending behavior.

## 6. Results

The K-Means algorithm successfully divided the customers into distinct groups based on their income and spending patterns.

The identified customer segments provide insights into different customer behaviors, such as:

* Customers with higher income and higher spending scores.
* Customers with higher income and lower spending scores.
* Customers with lower income and higher spending scores.
* Customers with lower income and lower spending scores.
* Customers with moderate income and moderate spending behavior.

The detailed characteristics and sizes of the clusters are presented in the corresponding analysis and visualization files.

## 7. Visualizations

### Dataset Information

![Dataset Information](screenshots/dataset_info.png)

### Gender Distribution

![Gender Distribution](screenshots/gender_distribution.png)

### Age Distribution

![Age Distribution](screenshots/age_distribution.png)

### Income Distribution

![Income Distribution](screenshots/income_distribution.png)

### Spending Score Distribution

![Spending Score Distribution](screenshots/spending_distribution.png)

### Elbow Method

![Elbow Method](screenshots/elbow_method.png)

### Customer Clusters

![Customer Clusters](screenshots/customer_clusters.png)

### Cluster Summary

![Cluster Summary](screenshots/cluster_summary.png)

### Cluster Sizes

![Cluster Sizes](screenshots/cluster_sizes.png)

## 8. Project Structure

```text
DataAnalytics-L1-CustomerSegmentation
│
├── Customer_Segmentation.ipynb
├──store_-customers.csv
├── README.md
│
└── screenshots
    ├── dataset_info.png
    ├── gender_distribution.png
    ├── age_distribution.png
    ├── income_distribution.png
    ├── spending_distribution.png
    ├── elbow_method.png
    ├── customer_clusters.png
    ├── cluster_summary.png
    └── cluster_sizes.png
```

## 9. Conclusion

This project demonstrates the application of unsupervised machine learning for customer segmentation using the K-Means Clustering algorithm. The analysis identifies groups of customers with similar income and spending characteristics.

The resulting customer segments can support businesses in understanding customer behavior, developing targeted marketing strategies, improving customer engagement, and making data-driven decisions.

## 10. Project Information

**Program:** OIBSIP Data Analytics Internship
**Task:** Customer Segmentation
**Machine Learning Technique:** K-Means Clustering
**Implementation:** Python and Jupyter Notebook

