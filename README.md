Customer Segmentation using Clustering
Overview
This project applies unsupervised machine learning to segment customers into distinct groups based on their demographic and behavioral attributes. 
By identifying customer clusters, businesses can design targeted marketing campaigns, optimize engagement, and improve overall strategy.

Dataset
Source: Mall Customer Segmentation Data (Kaggle)
Size: 200 customers
Features:
Age
Annual Income (k$)
Spending Score (1–100)

Project Workflow

Data Exploration → Dataset info, summary statistics, correlation heatmap
Preprocessing → Missing value handling, feature scaling
Dimensionality Reduction → PCA (2D) for visualization

Clustering
KMeans with Elbow Method (optimal k=4)
Gaussian Mixture Models (probabilistic clustering)
Evaluation → Compared models using Silhouette Score
Visualization → PCA scatter plots with clusters
Insights → Business-oriented cluster interpretations

Results
KMeans Silhouette Score: ~0.55
GMM Silhouette Score: ~0.42

KMeans performed better for this dataset.

Cluster Insights:
Cluster 1 → High income, high spend → Premium customers
Cluster 2 → High income, low spend → Potential customers
Cluster 3 → Low income, low spend → Budget-conscious
Cluster 4 → Young, moderate income, high spend → Trend-driven

Business Value
Helps identify premium customers for loyalty programs.
Detects under-engaged high-income customers.
Supports data-driven marketing segmentation.

Tech Stack
Python (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn)
Machine Learning: KMeans, Gaussian Mixture Models, PCA

How to Run

Clone the repository

git clone https://github.com/yourusername/customer-segmentation.git
cd customer-segmentation


Install dependencies
pip install -r requirements.txt


Run the script
python clustering.py

View the visualizations in the output plots.

Conclusion

This project demonstrates how unsupervised ML can provide actionable insights for businesses by segmenting customers.
Among the models tested, KMeans clustering produced the most meaningful segments, validated by Silhouette Score and visualization.
Feel free to use the code and make it better 
