# Customer Segmentation Using K-Means Clustering

## 📌 Overview

Customer Segmentation is the process of dividing a customer base into distinct groups based on similarities in behavior, interests, demographics, and spending habits. This segmentation allows businesses to target their marketing strategies more effectively. In this project, we use **K-Means Clustering** to segment mall customers based on their **Age**, **Annual Income**, and **Spending Score**.

---

## 🎯 Objectives

- To identify potential customer segments using clustering techniques.
- To understand customer behavior through visual analytics and statistical exploration.
- To build a machine learning model for effective customer grouping based on defined characteristics.

---

## 🧾 Dataset Description

- **Features:**
  - `CustomerID`: Unique identifier for each customer
  - `Gender`: Categorical (Male/Female)
  - `Age`: Integer (18–70)
  - `Annual Income (k$)`: Numeric (15–137)
  - `Spending Score (1–100)`: Numeric rating assigned based on customer behavior

---

## 🧪 Exploratory Data Analysis (EDA)

- **Gender Distribution:**  
  - Females: 112 (56%)  
  - Males: 88 (44%)  
  - Insight: Majority of mall customers are female.

- **Age Analysis:**
  - Age Range: 18–70 years
  - Most common age group: 30–50 years
  - Mean Age: ~35 years

- **Annual Income & Spending Score:**
  - Income Range: 15k–137k
  - Spending Score Range: 1–99
  - Highest density in the mid-income (60–75k) and mid-spending score (40–60) bands

---

## 📊 Clustering Technique – K-Means

- **K-Means Clustering:**  
  An iterative algorithm used to divide the dataset into K distinct, non-overlapping clusters.

- **Distance Metric:**  
  Euclidean Distance is used to assign data points to the closest cluster centroid.

- **Optimal K Selection:**  
  The **Elbow Method** was used to find the optimal number of clusters. Based on the WCSS plot, the ideal number of clusters is **5**.

---

## 🧩 Cluster Insights

1. **Cluster Green – Target Customers:**
   - High Income & High Spending
   - Primary focus for marketing and retention

2. **Cluster Red – Spenders:**
   - Low Income & High Spending
   - Spend more than they earn — still important

3. **Cluster Blue – Pitch Penny Customers:**
   - High Income & Low Spending
   - Potential to convert into higher spenders

4. **Cluster Purple – Normal Customers:**
   - Average Income & Spending
   - Neutral behavior, good for upselling strategies

5. **Cluster Orange – Balanced Customers:**
   - Low Income & Low Spending
   - Least attractive segment for promotions
  
     ![Cluster Plot](images/cluster_plot.png)

---

## 🛠 Technologies Used

- **Language:** Python
- **Environment:** Jupyter Notebook
- **Libraries:**
  - `Pandas`
  - `NumPy`
  - `Matplotlib`
  - `Seaborn`
  - `Scikit-learn`

---

---

## 📈 Results

- **Number of Clusters:** 5
- **Segmentation Outcome:** Successfully grouped customers into distinct behavioral segments
- **Business Value:** Enables targeted marketing, tailored product offerings, and improved customer satisfaction
