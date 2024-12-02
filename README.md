# Dimensionality Reduction Techniques

## **Overview**
This repository demonstrates various dimensionality reduction techniques on both image and tabular datasets. The primary aim is to understand and visualize how these methods work, compare their results, and discuss their effectiveness on different datasets.


### **1. Datasets**
1. **Image Data**
   - *Digits Dataset*: A collection of 8x8 grayscale images of digits (0-9) from `sklearn.datasets`.
   - *Olivetti Faces Dataset*: A dataset of 64x64 grayscale face images from `sklearn.datasets`.

2. **Tabular Data**
   - *Iris Dataset*: The classic Iris flower dataset with four features and three classes.
   - *Medical Dataset*: Pulled from Kaggle (e.g., diabetes or heart disease datasets).

---

### **2. Techniques Implemented**
Each technique is explained with theory, implemented using Python, and visualized interactively where applicable.

| **Technique**            | **Dataset**         | **Visualization**  |
|---------------------------|---------------------|---------------------|
| Randomized PCA            | Digits             | 2D Scatter Plot     |
| Kernel PCA                | Digits             | 2D Scatter Plot     |
| Incremental PCA           | Digits             | 2D Scatter Plot     |
| Locally Linear Embedding  | Olivetti Faces     | 2D Scatter Plot     |
| t-SNE                     | Iris               | Interactive Plot    |
| UMAP                      | Tabular (Medical)  | Interactive Plot    |
| ISOMAP                    | Olivetti Faces     | 2D Scatter Plot     |
| MDS                       | Tabular (Medical)  | 2D Scatter Plot     |
| Factor Analysis           | Tabular (Medical)  | 2D Scatter Plot     |
| Autoencoders              | Digits             | 2D Scatter Plot     |

---

### **3. Tools Used**
- **Libraries**: `scikit-learn`, `matplotlib`, `seaborn`, `umap-learn`, `keras`, `tensorflow`.
- **Interactive Visualizations**:
  - `plotly` for t-SNE and UMAP.
  - `ipywidgets` for interactive sliders to adjust parameters.

---

## **Results and Commentary**

1. **Digits Dataset**
   - PCA and t-SNE preserved clear digit clusters.
   - UMAP provided sharper clusters compared to t-SNE.
   - Autoencoders provided a compact and highly non-linear representation.

2. **Faces Dataset**
   - LLE captured local neighborhood structures better than PCA.
   - ISOMAP preserved global geometry and worked well for faces.

3. **Tabular Data**
   - Kernel PCA and t-SNE worked well for non-linear separability.
   - Factor Analysis failed to capture key variations in the medical dataset.

Youtube links:

1. Dimensionality_Reduction_Techniques_on_Tabular_Data: https://youtu.be/2mfE0YZwBUg
2. Dimensionality_Reduction_Techniques_Image_Data: https://youtu.be/Ln1zNJobIhc
