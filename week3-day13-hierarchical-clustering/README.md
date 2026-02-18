# Week 3 – Day 13  
## Hierarchical Clustering on Iris Dataset

### Objective
To perform hierarchical clustering using multiple linkage methods and analyze how linkage choice affects cluster formation and quality.

This assignment focuses on understanding tree-based clustering and comparing clustering performance using the Silhouette Score.

---

## Dataset
**Iris Dataset** (built into Scikit-learn)

The dataset contains 150 flower samples with the following features:

- Sepal Length
- Sepal Width
- Petal Length
- Petal Width

The goal is to group flowers into natural clusters without using labels (unsupervised learning).

---

## Tools & Libraries
- Python
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- SciPy

---

## Methodology

### 1. Data Preprocessing
- Dataset loaded from sklearn
- Features standardized using StandardScaler
- Scaling required because hierarchical clustering depends on distance

---

### 2. Dendrogram Construction
Dendrograms were generated using different linkage strategies:

- Single Linkage
- Complete Linkage
- Average Linkage
- Ward Linkage

These help determine cluster separation and appropriate cutting height.

---

### 3. Agglomerative Clustering
Clusters were created using:

AgglomerativeClustering(n_clusters = 3)

Each linkage method was tested separately.

---

### 4. Cluster Evaluation
Clustering quality evaluated using:

**Silhouette Score**

Higher score → Better separation between clusters

---

### 5. Cluster Visualization
Clusters plotted using Sepal Length vs Sepal Width to visually inspect separation.

---

## Results & Observations

| Linkage Method | Behaviour |
|--------------|------|
| Single | Produced chaining effect and weak separation |
| Complete | Formed compact clusters but some overlap |
| Average | Moderate separation |
| Ward | Best separation and most balanced clusters |

Ward linkage produced the highest silhouette score, indicating the most natural grouping.

---

## Key Learning

- Hierarchical clustering builds clusters step-by-step instead of partitioning data at once.
- Linkage choice significantly affects clustering output.
- Ward linkage minimizes intra-cluster variance, giving more meaningful clusters.
- Dendrograms help determine cluster structure before clustering.

---

## Files Included

- hierarchical_clustering.ipynb → Implementation notebook
- dendrogram_single.png
- dendrogram_complete.png
- dendrogram_average.png
- dendrogram_ward.png
- clusters_ward.png
- README.md

---

## Conclusion
Hierarchical clustering successfully grouped the Iris dataset into natural categories.  
Among all linkage methods, **Ward linkage performed best** due to variance minimization, producing compact and well-separated clusters.
