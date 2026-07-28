# Customer Segmentation & PCA Analysis – Epochs '26 Assignment 7

**Name:** [Nandhana S]  
**MUID:** [nandhanas-4@mulearn]  

---

## 📌 Business Objective
The goal of this project is to apply unsupervised learning techniques to segment mall customers based on demographics and spending behaviors. Using **K-Means Clustering** and **PCA Visualization**, we identify distinct customer groups to inform targeted marketing strategies.

---

## 📂 Dataset Overview
* **Dataset:** Mall Customer Segmentation Dataset
* **Features:** `Gender`, `Age`, `Annual Income (k$)`, `Spending Score (1-100)`
* **Pre-processing:** Categorical features encoded and normalized using `StandardScaler`.
* **Importance of Scaling:** K-Means relies on distance calculation (Euclidean distance). Features on larger scales (like income) can dominate distance calculations over smaller scale features (like age). Scaling ensures equal weight across features.

---

## 🛠️ Methodology & Modeling

1. **Optimal K Selection:** Evaluated `K` values from 1 to 10 using the Elbow Method (WCSS plot), identifying **K = 5** as the optimal cluster count.
2. **K-Means Clustering:** Trained K-Means model with $K=5$ and assigned each customer to a cluster.
3. **Dimensionality Reduction (PCA):** Applied PCA to project scaled features into 2 principal components to visualize the customer clusters in 2D space.

---

## 📊 PCA Variance & Visualizations
* **PCA Component 1 Variance Explained:** ~34%  
* **PCA Component 2 Variance Explained:** ~26%  
* **Total Variance Retained:** ~60%  

---

## 🏷️ Customer Segments & Business Recommendations

| Cluster | Segment Profile | Business Strategy |
| :---: | :--- | :--- |
| **0** | **Moderate Income / Low-Moderate Spending** | Focus on value offers, loyalty rewards, and discount promotions. |
| **1** | **High Income / Low Spending** | Market exclusive premium products; implement engagement campaigns to convert them to active buyers. |
| **2** | **High Income / High Spending (VIPs)** | Target for premium service, personalized marketing, early access to releases, and concierge loyalty programs. |
| **3** | **Low Income / Low Spending** | Offer budget-friendly essential items, seasonal sales, and bulk deals. |
| **4** | **Low Income / High Spending** | Target with trend-focused marketing and affordable impulse-buy items. |

---

## 🔮 Conclusions
Applying K-Means clustering combined with PCA successfully simplified complex multi-dimensional customer behavioral data into actionable business categories, allowing tailored customer strategies for maximized marketing ROI.
