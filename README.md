# Dimensionality Reduction Techniques

## **Overview**
This repository demonstrates the application of various dimensionality reduction techniques on both image and tabular datasets. The goal is to explore, visualize, and compare the results of these techniques, while also discussing their effectiveness when applied to different types of data.

---

### **1. Datasets**

#### **Image Data**
- **Digits Dataset**: A collection of 8x8 grayscale images representing digits (0-9) from `sklearn.datasets`.
- **Olivetti Faces Dataset**: A set of 64x64 grayscale images of faces from `sklearn.datasets`.

#### **Tabular Data**
- **Iris Dataset**: The classic Iris flower dataset, which includes four features and three classes.
- **Medical Dataset**: Data from Kaggle (e.g., diabetes or heart disease datasets).

---

### **2. Techniques Implemented**
Each dimensionality reduction technique is explained theoretically, implemented in Python, and visualized interactively where possible.

| **Technique**              | **Dataset**         | **Visualization**     |
|----------------------------|---------------------|-----------------------|
| Randomized PCA             | Digits             | 2D Scatter Plot       |
| Kernel PCA                 | Digits             | 2D Scatter Plot       |
| Incremental PCA            | Digits             | 2D Scatter Plot       |
| Locally Linear Embedding   | Olivetti Faces     | 2D Scatter Plot       |
| t-SNE                      | Iris               | Interactive Plot      |
| UMAP                       | Medical Dataset    | Interactive Plot      |
| ISOMAP                     | Olivetti Faces     | 2D Scatter Plot       |
| MDS                        | Medical Dataset    | 2D Scatter Plot       |
| Factor Analysis            | Medical Dataset    | 2D Scatter Plot       |
| Autoencoders               | Digits             | 2D Scatter Plot       |

---

### **3. Tools Used**
- **Libraries**: 
  - `scikit-learn`, `matplotlib`, `seaborn`, `umap-learn`, `keras`, `tensorflow`.
  
- **Interactive Visualizations**: 
  - `plotly` for t-SNE and UMAP.
  - `ipywidgets` for interactive sliders to adjust parameters.

---

## **Results and Commentary**

### **1. Digits Dataset**
- PCA and t-SNE preserved distinct clusters for the digits.
- UMAP produced clearer clusters compared to t-SNE.
- Autoencoders offered a compact, highly non-linear representation of the digits.

### **2. Faces Dataset**
- Locally Linear Embedding (LLE) effectively captured local neighborhood structures, performing better than PCA.
- ISOMAP maintained global geometry, showing good results with face images.

### **3. Tabular Data**
- Kernel PCA and t-SNE demonstrated strong performance on non-linearly separable data.
- Factor Analysis struggled to capture key variations, particularly in the medical dataset.


## Links to Demonstrations

### 1. [Dimensionality Reduction - Google Colab](https://github.com/subhashpolisetti/Dimensionality_Reduction/blob/main/Dimensionality_Reduction_Using_Databricks.ipynb)  
This notebook explores various dimensionality reduction techniques with interactive visualizations.

### 2. [Dimensionality Reduction - Databricks](https://github.com/subhashpolisetti/Dimensionality_Reduction/blob/main/Dimensionality_Reduction_Tabular_Data.ipynb)  
Scalable implementation of dimensionality reduction on Databricks for large datasets.

### 3. [Dimensionality Reduction for Images and Tabular Data](https://github.com/subhashpolisetti/Dimensionality_Reduction/blob/main/Dimensionality_Reduction_Tabular_Data.ipynb)  
Includes techniques applied on both image and tabular datasets, including medical datasets.

### 4. [Video Demonstration](https://drive.google.com/drive/folders/1rqq3_SqfZpaSAcj5LMMc0LiLdAQ1NRoP?usp=sharing)  
Watch the video demonstration of dimensionality reduction techniques and their applications.


