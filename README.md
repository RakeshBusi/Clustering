# Pipeline for Clustering Analysis of Protein Sequences

This repository contains a comprehensive pipeline for clustering protein sequences using various clustering algorithms. The pipeline includes data preprocessing, feature extraction, clustering, and evaluation of clustering performance.

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Preprocessing](#preprocessing)
- [Feature Extraction](#feature-extraction)
- [Clustering Analysis](#clustering-analysis)
- [Evaluation Metrics](#evaluation-metrics)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Introduction
Protein sequence clustering is a crucial task in bioinformatics, enabling the identification of protein families and functional annotation. This pipeline leverages multiple clustering algorithms to provide robust and accurate clustering of protein sequences.

## Dataset
- **Lysozyme CGCh Dataset**: Contains fasta files of Lysozyme C, Lysozyme G, and Lysozyme Ch protein families.
- **Labels**: Lysozyme C, Lysozyme G, and Lysozyme Ch.

## Preprocessing
- **Duplicate Removal**: Removes duplicate sequences within and between protein families.
- **Non-standard Amino Acid Elimination**: Eliminates sequences containing non-standard amino acids (UZOBJX).
- **Optional Outlier Removal**: Removes outliers based on sequence length.
- **Optional Length Filtering**: Filters sequences below a specified length threshold.

## Feature Extraction
- **Pseudo Amino Acid Composition (PAAC)**: Extracts features based on physicochemical properties of amino acids.
- **Physicochemical Properties Considered**:
  - Hydrophobicity
  - Hydrophilicity
  - Mass

## Clustering Analysis
Implements multiple clustering algorithms:
- KMeans
- Agglomerative Clustering
- Gaussian Mixture
- Spectral Clustering
- Affinity Propagation
- DBSCAN
- OPTICS
- Mean-shift
- BIRCH

## Evaluation Metrics
### Intrinsic Metrics
- **Silhouette Coefficient (SC)**
- **Calinski-Harabasz Index (CH)**
- **Davies-Bouldin Index (DB)**

### Extrinsic Metrics
- **Fowlkes-Mallows Index (FMI)**
- **F1 Score**
- **Matthews Correlation Coefficient (MCC)**
- **Adjusted Mutual Information (AMI)**
- **Contingency Matrix**

## Installation
To run this pipeline, you need Python 3.8+ and the following packages:
- numpy
- pandas
- scikit-learn
- matplotlib
- seaborn

You can install the required packages using:
```bash
pip install -r requirements.txt