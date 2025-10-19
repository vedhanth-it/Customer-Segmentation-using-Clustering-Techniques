# 🧩 Customer Segmentation and Pattern Discovery using Clustering Techniques

## 📘 Project Context
This project aims to perform **customer segmentation** based on behavioral and demographic patterns using **unsupervised machine learning**. By leveraging clustering algorithms, the goal is to group customers with similar characteristics to enable better marketing strategies and decision-making.

---

## 🧠 Problem Statement
Businesses often struggle to understand diverse customer groups due to high-dimensional and unstructured data.  
This project focuses on:
- Identifying hidden customer patterns.  
- Segmenting customers into meaningful clusters.  
- Comparing clustering methods (K-Means, Hierarchical, DBSCAN) for optimal segmentation.

---

## 📊 Data Information
- **Source:** Dataset containing customer purchase and demographic data.  
- **Type:** Mixed — both **categorical and numerical** variables.  
- **Key Features:** Year, Gender, Season, Article Type, and others related to customer activity and product characteristics.  
- **Goal Variable:** None (unsupervised task).  

---

## 🧹 Data Cleaning
Steps involved in data preparation:
1. Checked and removed **missing values**.  
2. Identified and dropped **duplicate rows**.  
3. **Dropped irrelevant columns** that didn’t contribute to clustering.  
4. Standardized **text formatting** (lowercase, trimmed spaces).  
5. Verified data consistency post-cleaning.

---

## 🔍 Exploratory Data Analysis (EDA)
- Analyzed **distributions** of numerical and categorical variables.  
- Studied **seasonal trends** and **gender-wise patterns**.  
- Visualized top categories such as **article types**, **seasons**, and **year-wise distributions**.  
- Created **heatmaps** to explore relationships (e.g., Season vs. Gender).

---

## ⚠️ Outlier Detection
- Used visual inspection via **boxplots** and **statistical summaries**.  
- Outliers were detected primarily in numerical features (e.g., spending patterns).  
- Depending on the algorithm, either handled or scaled to minimize distortion.

---

## ⚙️ Clustering Methods

### 1. **K-Means Clustering**
- Determined optimal `k` using:
  - **Elbow Method**
  - **Silhouette Score**
- Applied final K-Means model and labeled clusters.

### 2. **Hierarchical Clustering**
- Built **dendrograms** for visual inspection.  
- Evaluated clusters using linkage distance thresholds.

### 3. **DBSCAN**
- Tested density-based clustering to detect **non-linear** patterns and **noise points**.  
- Tuned `eps` and `min_samples` parameters.

---

## 🧩 Model Training and Evaluation
- Only **numeric and encoded** features were used for clustering.  
- Created an **evaluation function** to compare models using:
  - **Silhouette Score**
  - **Davies–Bouldin Index**
  - **Calinski–Harabasz Score**
- Compared cluster quality across K-Means, Hierarchical, and DBSCAN.

---

## 📈 Visualization
Visual insights included:
- **Elbow and Silhouette plots** for optimal cluster count.  
- **2D projections** of clusters using PCA/t-SNE.  
- **Heatmaps** and **bar plots** illustrating feature patterns by cluster.  
- Cluster characteristics summarized to interpret group behavior.

---

## 🧾 Conclusion
- Successfully segmented customers into **distinct behavioral clusters**.  
- **K-Means** provided the most balanced performance among methods.  
- Each cluster revealed **unique purchasing and seasonal traits**.  
- The analysis provides a foundation for **personalized marketing** and **targeted promotions**.

---

## 🚀 Future Work
- Apply **Gaussian Mixture Models (GMM)** for soft clustering.  
- Perform **feature importance analysis** for interpretability.  
- Integrate **real-time clustering dashboards**.
