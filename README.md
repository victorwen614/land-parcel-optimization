# 🌍 Land Parcel Optimization for Carbon Storage

## 📌 Overview

This project demonstrates the use of **geospatial data analysis** and **mathematical optimization** to select a subset of land parcels that **maximize carbon storage**, subject to:

- A total budget constraint (≤ 50% of total cost)
- No adjacency between selected parcels (no two selected parcels may share a boundary)
- (Optional) A minimum total area threshold (≥ 25% of total area)

The dataset includes 100 synthetic land parcels stored in a shapefile with attributes:
- `parcel_id` (unique identifier)
- `carbon_store` (float)
- `cost` (float)

---

## 🛠️ Environment Setup

You can create and activate the Python environment using conda:

```bash
conda create -n geo_opt python=3.10 -y
conda activate geo_opt
conda install -c conda-forge geopandas shapely pyproj pulp matplotlib pandas numpy -y
