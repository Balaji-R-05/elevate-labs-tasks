# Task 8: Clustering with K-Means

## Objective
Perform **unsupervised learning** using **K-Means clustering** to identify customer segments from a dataset. You'll learn how to use the **Elbow Method** and **Silhouette Score** to evaluate the optimal number of clusters.


## Dataset
**Mall Customer Segmentation Dataset**  
📎 [Kaggle Link](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python)


## Tools & Libraries Used
- Python
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- kneed (for automatic elbow detection)


## 🔍 Workflow

### 1. Data Preprocessing
- Dropped `CustomerID` as it has no predictive value.
- Encoded `Gender` column (Male → 1, Female → 0).
- Standardized all features using `StandardScaler`.

### 2. Visualize Dataset (Optional PCA)
- Used **PCA** to reduce dimensions for visualization.
- Plotted pairwise relationships to explore structure.

### 3. Elbow Method (Inertia)
- Calculated **inertia** (sum of squared distances to cluster centers) for k = 1 to 10.
- Plotted **inertia vs k**.
- Used `kneed` to automatically find the **elbow point**.

### 4. Final KMeans Clustering
- Chose optimal `k` from elbow method.
- Applied K-Means clustering.
- Visualized clusters using PCA-reduced 2D data.

### 5. Evaluation
- Calculated **Silhouette Score** to measure cluster cohesion and separation.
