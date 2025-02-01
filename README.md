# Advanced Customer Segmentation

## 📌 Project Overview
This project performs customer segmentation using **four clustering methods**:
- **K-Means**
- **DBSCAN**
- **Gaussian Mixture Model (GMM)**
- **Hierarchical Clustering**

The dataset used is **Mall Customers**, which contains customer demographic and spending behavior. This project incorporates advanced segmentation analysis techniques, high-dimensional distribution exploration, cluster validation, and interactive visualizations.

## 📂 Dataset
The dataset is retrieved from:
```
https://raw.githubusercontent.com/krishnaik06/Mall-Customers-Segmentation/master/Mall_Customers.csv
```
### Features Used:
- `Age`
- `Annual Income (k$)`
- `Spending Score (1-100)`

## 🛠 Steps in the Project

### 1️⃣ Advanced Exploratory Data Analysis (EDA)
- **3D Interactive Scatter Plot**: Visualizes customer distribution.
- **Pairplot with Density Estimation**: Identifies patterns across features.
- **Hierarchical Correlation Matrix**: Uses clustering to reveal feature relationships.

### 2️⃣ Data Preprocessing
- **Polynomial Features**: Captures non-linearity in data.
- **Standard Scaling & PCA**: Reduces dimensionality while preserving 95% variance.

### 3️⃣ Clustering Model Training & Hyperparameter Tuning
- **Grid Search Optimization** is applied to determine the best parameters for each clustering method.
- Metrics used for evaluation:
  - **Silhouette Score**
  - **Davies-Bouldin Index**
  - **Calinski-Harabasz Score**

### 4️⃣ Advanced Cluster Visualization
- **3D Cluster Comparison**: Compares clusters found by different models.
- **UMAP Projection**: Reduces dimensionality while preserving cluster structure.
- **SHAP Analysis**: Explains feature importance for each cluster.

### 5️⃣ Customer Segmentation Analysis
- **Cluster Profiling**: Summarizes demographic information per cluster.
- **Radar Chart**: Compares cluster characteristics in a visual format.

### 6️⃣ Stability Analysis & Deployment
- **Bootstrap Testing**: Measures cluster stability.
- **Deployment Pipeline**: Saves the best model (`Gaussian Mixture`) for production use.
- **Model Export**: Final pipeline saved as `customer_clustering_pipeline.pkl`.

## 🔧 Requirements
Install required dependencies using:
```bash
pip install numpy pandas matplotlib seaborn scikit-learn plotly yellowbrick shap umap-learn joblib
```

## 🚀 Running the Project
Run the clustering pipeline with:
```bash
python clustering_expert.py
```

## 📌 Results
- Gaussian Mixture Model (GMM) was found to be the best clustering method.
- Identified customer segments based on their spending and income characteristics.
- Deployed a ready-to-use clustering pipeline for future customer segmentation tasks.

---

