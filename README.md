# MODIS LULC Frequency and Area Analysis (ArcPy)

This repository contains a Python script that performs area and frequency analysis on a classified MODIS 500m LULC raster. It converts the raster to polygons, calculates areas (in km²), aggregates category frequencies, and computes percentage coverage.

## 🔧 Features
- Converts raster to integer and polygon
- Calculates area in square kilometers
- Aggregates land cover class frequency
- Calculates % of each class from total
- Outputs a frequency table (.dbf)

## 📁 Input
- Classified MODIS LULC raster (e.g., 500m resolution GeoTIFF)
  
## 📂 Output
- Polygon shapefile with area field
- `.dbf` table of category area/frequency
- Console summary

## 🛠 Requirements
- Python 3.x
- ArcPy (ArcGIS Pro or Desktop)
- Spatial Analyst extension

## 📌 Usage
1. Update the following paths in the script:
   ```python
   workspace = r"Path\\to\\your\\workspace"
   input_raster = "YourLULCfile.tif"
   output_path = r"Path\\to\\output"
   python modis_lulc_analysis.py

