# Lecture 04 — Enhanced K-means Clustering Teaching Example

**Module:** OMC9000UK7 — Principles and Applications of Artificial Intelligence and Machine Learning.  
**Course alignment:** Lecture 04, MLO1 and MLO3.  
**Source:** Lecturer-supplied `Kmean Clustering.ipynb` and `Kmean2.csv`.

## Files

- `KMeans_Clustering_Enhanced.ipynb` — expanded, fully executed Jupyter notebook with explanations and **10 embedded visualisations**, plus exercises and citations.
- `KMeans_Clustering_Enhanced_Illustrated.html` — static illustrated version of the notebook, useful for students without Python.
- `Kmean2_original.csv` — all **33 original coordinates**; original numerical content preserved.
- `Kmean2_improved.csv` — **343** examples: the original 33 plus **310 newly simulated points** in five groups; column `source` distinguishes them.
- `cluster_assignments.csv` — fitted K-means labels for the 343 teaching examples.
- `cluster_centroids.csv` — trained centroid coordinates and cluster sizes.
- `Elbow_and_Silhouette.png`, `KMeans_Clusters_and_Centroids.png`, `New_Point_Predictions.png` — selected figures for presentations/teaching.

## Quick start

```bash
python -m pip install numpy pandas matplotlib scikit-learn jupyter
jupyter notebook KMeans_Clustering_Enhanced.ipynb
```

Keep the notebook and CSVs in the same directory. Run cells in order or use **Run All**. The notebook was fully executed and the outputs were saved before delivery.

## Teaching outcomes

The notebook builds from **one manual iteration** of centroid assignment/update to choosing K via elbow/silhouette, fitting scikit-learn's KMeans, profiling clusters, evaluating structure, interpreting new points, checking stability and discussing scaling.

## Validated example metrics (synthetic teaching dataset)

- Number of observations: **343**
- Clusters used: **5**, also the best silhouette choice among K=2–9 for this simulated example.
- Silhouette coefficient: **0.803**
- Davies–Bouldin index: **0.272**
- Inertia on standardised features: **13.48**

**Important:** This is *unsupervised* clustering on generic two-dimensional coordinates, not a real-world dataset with known ground-truth classes. Classification metrics such as accuracy, precision, recall and confusion matrix do **not** apply without independent reference labels. Do not infer real-world predictive validity from a synthetic example. K-means group identifiers have no intrinsic interpretation.

## What was changed from the original notebook?

The original 7-cell notebook loaded 33 points, ran KMeans(k=5), and plotted clusters, with some points joined by lines. The revision adds pedagogy, reproducibility, correct scatter-only plotting, simulated extension provenance, data checks, scaler, K choice, evaluation, centroids and new-point predictions.
