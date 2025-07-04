# 🧠 Customer Segmentation using K-Means Clustering & PCA

This project focuses on **segmenting customers** into meaningful groups based on their behavior using **unsupervised machine learning** techniques like **K-Means clustering** and **Principal Component Analysis (PCA)**.

---

## 📁 Dataset

- **Source**: [Kaggle - Mall Customer Dataset]
- **Rows**: ~2240 customers  
- **Features**: Age, Gender, Income, Spending Score, and more

---

## 🛠️ Technologies Used

- Python 3  
- Pandas & NumPy  
- Scikit-learn  
- Matplotlib  
- Seaborn (optional for enhanced visuals)

---

## 📌 Project Workflow

### ✅ 1. Data Preprocessing
- Handled missing values in `Annual Income` (filled with mean)
- Converted `dt_customer` column to datetime
- Extracted `days_since_joining` as a feature
- Label encoded categorical variables like `Gender`

### ✅ 2. Feature Scaling
- Used `StandardScaler` to normalize all features for PCA & K-Means

### ✅ 3. Dimensionality Reduction (PCA)
- Applied PCA to reduce 29 features to 23 while preserving ~95% of variance
- Used 2 principal components for 2D cluster visualization

### ✅ 4. Optimal Cluster Selection
- Applied **Elbow Method** to find best `k`
- Verified with **Silhouette Score**
- Chose **k = 3** clusters based on performance and interpretability

### ✅ 5. Clustering (K-Means)
- Fitted KMeans with `n_clusters=3`
- Assigned each customer to a cluster
- Visualized cluster groups using PCA

---

## 📊 Visual Output

- **Elbow Plot** for optimal k  
- **Silhouette Score** comparison  
- **2D scatter plot** of customer clusters

---

## 📁 Output

- Labeled DataFrame with `Cluster` column
- Visual segmentation of customers
- Ready-to-use CSV for further analysis or marketing targeting

---
