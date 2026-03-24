# Self-Organizing Map (SOM) Tutorial with Iris Dataset

## Overview
This repository contains a complete tutorial on **Self-Organizing Maps (SOMs)**, demonstrating unsupervised learning and feature visualization using the **Iris dataset**. The tutorial focuses on building intuition for SOMs, visualizing the U-Matrix, component planes, and cluster assignment, and provides a hands-on implementation entirely in Python using **NumPy** and **Matplotlib**.

The project is designed as an **educational tutorial**, suitable for students, researchers, and anyone interested in neural network-based unsupervised learning.

---

## Contents

- `figures/` – Folder containing all generated figures:
  - `som_u_matrix.png` – U-Matrix showing distance between SOM nodes.
  - `som_labels_overlay.png` – SOM with Iris labels overlay.
  - `component_plane_0.png` … `component_plane_3.png` – Feature-specific component planes.
  - `cluster_map.png` – Cluster assignment map.
- `som_tutorial.ipynb` – Jupyter Notebook with full code and explanations.
- `webpage/index.html` – Web-based tutorial version (<2000 words).
- `README.md` – This file, describing the repository and instructions.
- `LICENSE` – MIT License to allow reuse.

---

## Learning Objectives
By using this repository, learners will:

1. Understand the concept of **Self-Organizing Maps** as unsupervised neural networks.
2. Explore **U-Matrix visualization** to understand cluster boundaries.
3. Analyze **component planes** for each feature in the dataset.
4. Generate **cluster assignment maps** to interpret SOM output.
5. Learn to implement SOM **from scratch in Python** without specialized packages.
6. Create **accessible and colorblind-friendly visualizations** for educational use.

---

## Dataset
We use the classical **Iris dataset** from [Scikit-learn](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_iris.html). It contains:

- 150 samples
- 4 features: Sepal length, Sepal width, Petal length, Petal width
- 3 target classes: Setosa, Versicolor, Virginica

Data is standardized using **z-score normalization** to ensure features contribute equally to SOM training.

---

## SOM Implementation

### Parameters
- Grid size: 7 × 7
- Input length: 4 (features)
- Learning rate: 0.5
- Sigma (neighborhood radius): 1.0
- Iterations: 1000

### Key Steps
1. **Weight Initialization:** Randomly initialize SOM weights.
2. **Best Matching Unit (BMU) Selection:** Find node closest to a sample.
3. **Neighborhood Update:** Update BMU and surrounding nodes using a Gaussian function.
4. **Visualization:** U-Matrix, component planes, label overlay, cluster map.

---

## Usage Instructions

1. Clone the repository:

```bash
git clone https://github.com/YourUsername/SOM-Tutorial-Iris-Dataset.git
cd SOM-Tutorial-Iris-Dataset
