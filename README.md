# FMCG Customer Segmentation

## Overview

This project provides a customer segmentation approach including business recommendations as a sample project for FMCG customer data.

Customer segmentation is the process of dividing customers into groups based on common characteristics so companies can market to each group effectively and appropriately. It can be employed by all types of business, regardless of size, industry and whether they sell online or in person. For example, a small business selling guitars might decide to promote lower-priced products to younger guitarists and higher-priced premium guitars to older musicians based on segment knowledge which tells them that younger musicians have less disposable income than their older counterparts.  
Generally, customer segmentation can help to personalise marketing efforts which has the potential to increase revenue, reduce customer churn, increase marketing efficiency through higher conversion rates, and to improve customer experience. Hence this report aims at segmenting 2000 FMCG customers such that recommendations can be derived to support the abovementioned goals.

## Exploratory Data Analysis

To better understand the customer base, the data is visualised using appropriate charts.

![EDA Plot](https://github.com/felix-rosenberger/customer-segmentation/blob/main/data/eda_plot_individual_features.png)

Note: an increase in numbers correlates with an increase in the categorical variable, i.e., larger city, more education, more highly skilled. Details can be found in the notebook.

## Insights

This report shows insights by exploring customer characteristics and applying two clustering techniques. To visualise the respective clusters in an informative way, two approaches were chosen:
1. Visualisation of cluster mean deviation from overall mean for each customer characteristic
2. Visualisation of feature distribution within each cluster using Box Plots

These visualisations allow intuitive understanding about 1) differences between clusters, 2) differences between clusters and overall customer base, and 3) distributions of characteristics within clusters.

### KMeans Results

![Cluster Characteristics Plot](https://github.com/felix-rosenberger/customer-segmentation/blob/main/data/cluster_mean_deviations.png)

![Cluster Characteristics Distributions Plot](https://github.com/felix-rosenberger/customer-segmentation/blob/main/data/kmeans_feature_dist.png)

- Cluster 1: mostly male and high school educated customers who are younger than 50 years (see Figure 6) with highly regarded occupation types, mostly living in big cities, and earning slightly above average.
- Cluster 2: mostly older than 50-year-old (see Figure 6) customers who are highly educated, mostly working as skilled employees, and earning mid to top income.
- Cluster 3: high school educated customers across a wide age range (see Figure 6), mostly unemployed/unskilled, almost entirely living in small cities, and earning low to mid income.

### Agglomerative Clustering Results

![Cluster Characteristics Plot](https://github.com/felix-rosenberger/customer-segmentation/blob/main/data/agglo_cluster_mean_deviations.png)

- Cluster 1: Mostly middle-aged male customers with high school or university education, working in highly qualified occupations, living in big cities, and earning top income.
- Cluster 2: Mostly younger customers with high school education, working either as skilled employee or are unskilled/unemployed, living in small to mid-sized cities, and earning slightly below average.
- Cluster 3: Old customers with a graduate school education, working in unskilled occupations or are unemployed, living in small to mid-sized cities, and earning average income.

### Recommendations

Based on the segmentation derived, the following recommendations are made for the respective customer segments.
<br>

- **Customers living in small cities, mostly unemployed with high school education:**
    - Budget-friendly product assortments
    - Loyalty programs and discounts
- **Older customers, highly educated, high income:**
    - Targeting for premium products like special wines, meats, fresh pasta etc.
    - Targeting for premium services like food delivery
- **Young customers, highly regarded occupation types, living in big cities:**
    - Cater to their busy and independent lifestyle by offering discounts on order delivery to increase retention rates. This gives big opportunities to increase the customer lifetime value as these customers are young and it is important that they stay loyal.
    - Enhance in-app experience, e.g. through gamification, to increase customer experience
    - Target these customers with healthy and regional products that are easy to make as these are most likely their preferences. However, this should be tested, e.g. through A/B testing.
    - Also focus on initiatives that enhance the brand like the reduction on food waste
