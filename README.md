# Wheat Seeds Data Mining: PCA, Clustering & LDA 🌾

## 📌 Project Overview
This project focuses on the exploratory data analysis and dimensionality reduction of geometric properties of three different varieties of wheat seeds. The goal is to cluster the seeds based on their features and predict their varieties using advanced Data Mining techniques in **R**.

## 🛠️ Techniques & Tools Used
* **Language:** R
* **Libraries:** `tidyverse`, `cluster`, `factoextra`, `MASS`, `GGally`, `ggplot2`
* **Dimensionality Reduction:** Principal Component Analysis (PCA)
* **Unsupervised Learning (Clustering):** * K-Means Clustering (evaluated via Elbow Method, Gap Statistic, Silhouette)
  * Hierarchical Clustering (Ward's Method, Complete Linkage)
* **Supervised Learning:** Linear Discriminant Analysis (LDA)

## 📊 Key Findings
1. **PCA:** We successfully reduced the dataset's dimensionality, with the first two Principal Components explaining almost **90% of the total variance**. PC1 captured the "Size" of the seed, while PC2 captured its "Shape".
2. **Clustering:** Both K-Means and Ward's Hierarchical Clustering identified **3 optimal clusters**, perfectly aligning with the 3 real seed varieties. Performing clustering on the PCA-reduced dataset yielded tighter, more homogeneous clusters with lower intra-cluster variance.
3. **LDA:** The Linear Discriminant Analysis model achieved a high prediction accuracy, misclassifying only a small fraction of seeds (approx. **3.3% error rate**).

## 📂 Repository Structure
* `Wheat_Seeds_Analysis.Rmd`: The complete R Markdown source code.
* `Wheat_Seeds_Analysis.html`: The rendered HTML report containing all plots, mathematical explanations, and comments. **(Recommended for viewing)**
* `data/`: Contains the original dataset (`semi_dataset.xlsx`).

## 🚀 How to Run
Clone the repository and open the `.Rmd` file in RStudio. Ensure you have the required packages installed. The data path is set relatively, so it should run out-of-the-box.
