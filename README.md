# DATA420 Assignment 2 — The Million Song Dataset

This repository contains my submission for **Assignment 2** in **DATA420 (2025 Semester 1)**.  
The assignment explores large-scale music data processing, classification, and recommendation systems using the **Million Song Dataset (MSD)**.

## 📄 Contents

- `notebook.ipynb`  
  Jupyter notebook containing all data exploration, preprocessing, modeling, and evaluation code.

- `report.pdf`  
  Final written report (PDF), describing methodology, results, and discussion in detail.

> **Note:** Large datasets and generated outputs are not included in this repository, as all data processing was performed directly in cloud storage.

---

## 🎵 Assignment Overview

The aim of this assignment was to analyse and model data from the **Million Song Dataset (MSD)** using distributed computing tools. The work is split into three major components:

### 1. Data Processing
- Exploration of MSD metadata, audio feature datasets, and user-song play counts
- Schema inference and structured loading of large datasets
- Systematic column naming for merging multiple audio feature sources
- Use of Spark and cloud storage (Azure Blob Storage)

### 2. Audio Similarity & Genre Classification
- Feature engineering using audio-based descriptors
- Binary genre classification (Electronic vs non-Electronic)
- Multiclass genre classification
- Models implemented using `spark.ml`, including:
  - Logistic Regression
  - Random Forest
  - Gradient-Boosted Trees (GBT)
- Evaluation using appropriate performance metrics and discussion of class imbalance

### 3. Song Recommendation System
- Collaborative filtering using implicit user-song play counts
- Data filtering to remove low-activity users and songs
- Model training with **Alternating Least Squares (ALS)**
- Evaluation using ranking metrics:
  - Precision@K
  - Mean Average Precision (MAP)
  - Normalised Discounted Cumulative Gain (NDCG)
- Discussion of real-world deployment considerations

---

## 🧰 Technologies Used

- **Python**
- **Apache Spark (PySpark)**
- **Spark MLlib**
- **Jupyter Notebook**
- **Azure Blob Storage**
- **HDFS-style distributed data access**

---

## 📊 Dataset

The analysis uses subsets of the **Million Song Dataset**, including:
- Audio feature datasets (Marsyas, jMir, MFCCs, spectral features)
- MSD Allmusic Genre Dataset (MAGD)
- Taste Profile Dataset (implicit user-song play counts)

Due to size and licensing constraints, the datasets are **not included** in this repository.

---

## 📌 Notes on Reproducibility

This repository is intended as a **portfolio and code reference**, not a fully reproducible pipeline:
- Data paths are specific to the university cloud environment
- Outputs are intentionally excluded
- Some cells assume access to pre-configured Spark clusters

---

## 📚 Academic Context

This work was completed as part of a formal university assessment.  
All analysis, interpretations, and written material are my own, completed in accordance with course academic integrity guidelines.
