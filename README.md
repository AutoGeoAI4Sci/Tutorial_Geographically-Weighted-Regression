# 📊 Tutorial: Geographically Weighted Regression (GWR)

Guest lecture materials for **GEOG 475: Advanced GIS**  
**Texas A&M University**

---

## 🔎 Overview

This repository provides a concise introduction to **Geographically Weighted Regression (GWR)**—a spatial regression technique designed to capture **local variation** in relationships (i.e., spatial non-stationarity).

GWR extends global regression by allowing model parameters (coefficients) to vary across geographic space, helping reveal spatially heterogeneous processes.

---

## 🧭 Table of Contents

- [What is GWR?](#-what-is-gwr)
- [Key Concepts](#-key-concepts)
- [Recommended Resources](#-recommended-resources)
- [Suggested Repository Structure](#-suggested-repository-structure)
- [Example Use Cases](#-example-use-cases)
- [Citation](#-citation)

---

## 📘 What is GWR?

**Geographically Weighted Regression (GWR)** is a spatial statistical method that:

- Estimates **location-specific** regression coefficients  
- Accounts for **spatial non-stationarity** (relationships vary across space)  
- Produces **local parameter surfaces** and **diagnostic outputs** (e.g., local R²)

GWR is widely used in geography, environmental science, urban studies, public health, and related fields.

---

## 🧠 Key Concepts

### 1) Spatial Non-Stationarity
Traditional regression assumes relationships are constant across space.  
GWR relaxes this assumption by modeling how relationships vary **locally**.

### 2) Kernel Weights
At each location, observations are weighted by distance using a spatial kernel function, such as:

- Gaussian
- Bisquare

### 3) Bandwidth Selection
Bandwidth controls the spatial scale of “locality” and strongly affects results.

Common strategies include:

- AICc-based selection
- Cross-validation (CV)

### 4) Local Diagnostics
GWR can output spatial surfaces of:

- Local coefficients
- Local R² / model fit
- Residuals and influence diagnostics

---

## 📚 Recommended Resources

### ESRI / ArcGIS Pro Documentation
- **How Geographically Weighted Regression (GWR) works (ArcGIS Pro)**  
  https://pro.arcgis.com/en/pro-app/latest/tool-reference/spatial-statistics/how-geographicallyweightedregression-works.htm

### Academic Overview
- **Geographically Weighted Regression (ScienceDirect topic page)**  
  https://www.sciencedirect.com/topics/earth-and-planetary-sciences/geographically-weighted-regression

### Technical Guide (PDF)
- **GWR Technical Guide (University of Bristol, PDF)**  
  https://www.bristol.ac.uk/media-library/sites/cmpo/migrated/documents/gwr.pdf

---

## 🗂 Suggested Repository Structure

You can organize your lecture materials like this:

```text
Tutorial_Geographically-Weighted-Regression/
├── slides/
│   └── GEOG475_GWR_GuestLecture.pdf
├── notes/
│   ├── 01_overview.md
│   ├── 02_key_concepts.md
│   └── 03_interpretation.md
├── demos/
│   ├── arcgis_pro_workflow.md
│   ├── pysal_mgwr_demo.ipynb
│   └── example_data/
└── README.md
````

---

## 🧪 Example Use Cases

| Field                 | Example Application                                 |
| --------------------- | --------------------------------------------------- |
| Urban Studies         | Modeling spatially varying housing price drivers    |
| Public Health         | Identifying local risk factors for disease outcomes |
| Environmental Science | Mapping local pollutant–health associations         |
| Transportation        | Local determinants of congestion or accessibility   |

---

## 📝 Citation

If you use or reference GWR in academic work, consider citing:

Brunsdon, C., Fotheringham, A. S., & Charlton, M. (1996).
*Geographically Weighted Regression: A Method for Exploring Spatial Non-Stationarity.*
**Geographical Systems**, 8, 161–185.
