# NISAR Forest Cover and Soil Moisture Analysis

![Image](https://github.com/user-attachments/assets/dcd0e1a5-eb45-462a-8bda-2bbdb0a64849)

---

## Overview
This project focuses on analyzing **NASA–ISRO SAR (NISAR)** data for:
1. **Forest cover mapping** using **L-band SAR HH and HV polarizations**
2. **Soil moisture analysis** using NISAR soil moisture products

---

## Objectives
- Analyze the sensitivity of **HH and HV polarizations** for forest cover mapping
- Generate forest-related backscatter metrics from NISAR GCOV products
- Explore **NISAR Soil Moisture (SM)** products for surface moisture assessment

---

## Data Used

### 1. NISAR SAR Data (GCOV)
- **Frequency:** L-band
- **Product:** GCOV (Geocoded Covariance)
- **Polarizations analyzed:**
  - HH (Horizontal transmit – Horizontal receive)
  - HV (Horizontal transmit – Vertical receive)

**Why HV?**
- **HV:** Strong indicator of volume scattering from vegetation canopy, highly useful for forest structure analysis

---

### 2. NISAR Soil Moisture Product
- **Product Type:** Level-3 Soil Moisture
- **Parameter:** Surface soil moisture

---

## Methodology

### Forest Cover Analysis
1. Extract HH and HV backscatter from NISAR GCOV HDF5 files
2. Convert backscatter values to **decibel (dB) scale**
3. Apply spatial masking for the study area
4. Analyze:
   - HV backscatter response
5. Visualize spatial patterns of forest cover and non forest cover

---

### Soil Moisture Analysis
1. Read NISAR soil moisture product
2. Extract surface soil moisture layers
3. Apply quality masking (if applicable)
4. Visualize spatial distribution of soil moisture

---

## Tools & Libraries
- Python
- `h5py`
- `xarray`
- `rioxarray`
- `numpy`
- `geopandas`
- `matplotlib`

---

## Author
**Sanjay M**  
GIS Specialist 
