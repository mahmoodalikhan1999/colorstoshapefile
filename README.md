

### **README for Color Detection and Shapefile Generation Tool**

# Color Detection & Shapefile Generator

This project processes GeoTIFF satellite images to detect specific colors, apply masks, and generate shapefiles for GIS analysis. The tool uses clustering techniques and color filtering to detect, mask, and visualize color segments for further geospatial analysis.

---

### **Features**
- **Color Detection:** Identifies specific colors in satellite images using tolerance-based color matching.
- **Color Masking:** Applies masks to visualize and extract specific color regions.
- **Shapefile Generation:** Creates and exports shapefiles of detected color regions for GIS applications.
- **Visualization:** Displays masked images for visual inspection.

---

### **Installation**

Ensure you have Python installed and run the following commands to set up the environment:

```bash
pip install rasterio webcolors numpy opencv-python matplotlib scikit-learn geopandas
```

---

### **Usage**

1. **Load Satellite Image**  
   Place your GeoTIFF image in the project directory and specify the path in the script:
   ```python
   image_path = "path_to_your_image.tif"
   ```

2. **Define Desired Colors and Tolerance**
   Customize the color detection by specifying the desired RGB values and tolerance level:
   ```python
   desired_colors = [(40, 106, 9), (113, 160, 90)]  # Example colors
   tolerance = 10  # Adjust as needed
   ```

3. **Run the Script**  
   Execute the notebook or script to process the image, generate masks, and export shapefiles.

4. **Output**  
   The masked image will be displayed, and the shapefile will be saved to the specified location:
   ```
   ./Updated_Shapefiles/Green_Calcite.shp
   ```

---

### **Visualization**

The project includes functions to:
- Mask non-matching colors in the image.
- Visualize the masked image with `matplotlib`.
- Display clusters of colors and their names using KMeans clustering.

---

### **Dependencies**
- **Python 3.6+**
- **Required Libraries:**  
  - `rasterio`
  - `webcolors`
  - `numpy`
  - `opencv-python`
  - `matplotlib`
  - `scikit-learn`
  - `geopandas`

---

### **License**
This project is open-source and available for modification and distribution.

---
