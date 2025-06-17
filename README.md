# 🌿 NDVI Vegetation Mapping – Pohjois-Savo, Finland

This project calculates and visualizes NDVI (Normalized Difference Vegetation Index) across the Pohjois-Savo region using **Landsat 8 Surface Reflectance** data. It demonstrates how satellite imagery and open-source geospatial tools can be used to assess vegetation density.

## 📍 Objective

To generate an accurate NDVI map of Pohjois-Savo using Python and QGIS, highlighting forested vs. open land areas.

---

## 🛠 Tools & Libraries Used

- **Satellite Data**: Landsat 8 Surface Reflectance (from USGS EarthExplorer)
- **Python Libraries**:  
  `Rasterio`, `GeoPandas`, `Shapely`, `Matplotlib`, `NumPy`
- **GIS Software**:  
  `QGIS` (for final visualization and validation)

---

## 🧪 Methodology

1. **Data Download**  
   - Landsat 8 SR bands retrieved from USGS EarthExplorer

2. **NDVI Calculation**  
   - Used Band 5 (NIR) and Band 4 (Red):  
     `NDVI = (NIR - Red) / (NIR + Red)`

3. **Region Clipping**  
   - Created a custom GeoJSON boundary for Pohjois-Savo
   - Clipped raster data to this boundary using `Rasterio`

4. **Visualization**  
   - Styled NDVI output with custom colormap
   - Cross-validated results using QGIS

---


