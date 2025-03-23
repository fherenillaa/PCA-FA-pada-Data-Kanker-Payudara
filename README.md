# 📊 PCA Analysis on Breast Cancer Wisconsin Dataset

This project performs Principal Component Analysis (PCA) on the Breast Cancer Wisconsin (Diagnostic) dataset to reduce dimensionality and visualize the main contributing features to classification.

## 📁 Dataset Description

The dataset used in this project was originally collected by **Dr. William H. Wolberg** at the **University of Wisconsin Hospitals, Madison**. It consists of digitized images of fine needle aspirate (FNA) of breast mass and describes characteristics of the cell nuclei present in the images.

- **Total Observations**: 569
- **Features**: 30 numeric features (mean, standard error, and worst of 10 real-valued features for each cell nucleus)
- **Target**: Diagnosis (`B` = Benign, `M` = Malignant)

## ⚙️ Methods

- **Principal Component Analysis (PCA)** was used to:
  - Reduce the dimensionality of the dataset
  - Identify key features contributing to variance
  - Visualize data in 2D using biplots

## 📈 Results

- **Component 1 (Dim1)** explains **43.5%** of the variance.
- **Component 2 (Dim2)** explains **14.6%** of the variance.
- **Cumulative Variance (Dim1 + Dim2)**: **58.1%**

### 🔎 Interpretation

The biplot illustrates how original variables contribute to the first two principal components. Features such as:
- `concave_points2`
- `compactness2`
- `concavity2`

...have strong influence on **Dim1**, which contributes most to the separation of data points (possibly between benign and malignant tumors).

## 📦 Files Included

| File Name            | Description |
|---------------------|-------------|
| `pca_analysis.Rmd`  | R Markdown source file for the analysis |
| `pca_analysis.html` | Rendered HTML report (published on Rpubs) |
| `data.csv`          | Breast cancer dataset used |
| `pca_biplot.png`    | PCA biplot visualization |
| `README.md`         | This file |

## 🌐 Rpubs Report

You can view the full interactive report here:  
👉 [**Rpubs Link**](https://rpubs.com/ismatul123/1287969)  

## 🧠 Requirements

- R version 4.x or higher
- R packages:
  - `factoextra`
  - `ggplot2`
  - `dplyr`
  - `tidyr`

Install with:

```r
install.packages(c("factoextra", "ggplot2", "dplyr", "tidyr"))
