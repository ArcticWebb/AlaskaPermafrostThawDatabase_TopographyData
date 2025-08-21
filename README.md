# Topographic Variable Extraction for the Alaska Permafrost Thaw Database

**Author:** Hailey Webb (hailey.webb@colorado.edu)  
**Date:** 2025-08-21 

## Description
This Google Earth Engine (GEE) script extracts and computes topographic variables for permafrost thaw database points using the 2m mosaic ArcticDEM.  

**Variables extracted:**
- Elevation
- Slope
- Aspect
- Relative elevation (point elevation minus mean elevation in 100 m buffer)
- Solar Radiation Index (SRI) at summer solstice noon

---

## Input
- Alaska permafrost thaw database points (shapefile)  
- ArcticDEM V4, 2 m mosaic

---

## Output
- CSV file exported to Google Drive containing thaw database points with appended topographic variables.

---

## Usage
1. Open the script in the **Google Earth Engine Code Editor**.  
2. Import the thaw database points and define export path.  
3. Run the script.  
4. Download the exported CSV.  

---

## Requirements
- Google Earth Engine account  
- Access to ArcticDEM dataset (UMN/PGC/ArcticDEM/V4/2m_mosaic)

---

## Notes
- This script assumes point geometries for the thaw database.
- Relative elevation is calculated using a 100 m buffer around each point.  
- SRI is computed using the methods outlined in Fu and Rich (2002) (https://doi.org/10.1016/S0168-1699(02)00115-1). Solar zenith angle is calculated using the latitude of individual thaw features.

---

## License
This script is released under the MIT License. Feel free to use, modify, and distribute with attribution.  

---

## Citation
Webb, H. (2025). *Topographic Variable Extraction for Alaska Permafrost Thaw Database* [GEE script]. GitHub. DOI via Zenodo.  
