# Drought Analysis using Standard Vegetation Index (SVI)

![SVI Image](https://github.com/DomWatcharin/Drought-Analysis-using-SVI/blob/9778818880daadda2a1aa8cbe42e44caf45fb262/SVI/SVI.png)

![Drought Analysis Image](https://github.com/DomWatcharin/Drought-Analysis-using-SVI/blob/9778818880daadda2a1aa8cbe42e44caf45fb262/SVI/Drought%20Analysis.png)

This repository contains Python scripts for detecting drought conditions in rice fields using satellite imagery. The scripts utilize geospatial data processing libraries such as GeoPandas and Rasterio to analyze Standard Vegetation Index (SVI) data within rice field polygons.

## Scripts

1. **Retrieving and Processing MODIS EVI Data**: This script retrieves and processes MODIS Enhanced Vegetation Index (EVI) data. It filters the data based on a specified time range and area of interest (AOI), applies cloud masking, and exports the processed EVI data as GeoTIFF images.

2. **Exporting Soil Vegetation Index (SVI) GeoTIFF**: This script exports SVI GeoTIFF images by reprojecting EVI data to a new coordinate reference system (CRS) and rearranging SVI values to a specified range.

3. **Plot Rice Field Polygons**: This script plots rice field polygons from a GeoJSON file using Matplotlib. It visualizes the polygons on a map for spatial reference.

4. **Reproject GeoTIFF to New Coordinate Reference System**: This script reprojects a GeoTIFF file to a new CRS specified by the user using the Rasterio library.

5. **Plotting Standard Vegetation Index (SVI) GeoTIFF**: This script plots SVI GeoTIFF files using Matplotlib. It visualizes the SVI data with a specified color palette.

6. **Detect Drought in Rice Fields using Satellite Data**: This script detects drought conditions in rice fields using SVI data. It calculates the mean SVI within each rice field polygon and identifies polygons with SVI values below a specified threshold.

## Usage

1. Ensure you have Python installed on your system.
2. Install the required Python packages: `geopandas`, `rasterio`, `numpy`, `matplotlib`.
3. Clone this repository to your local machine.
4. Navigate to the repository directory and run the desired script.

```bash
python SVI.py
