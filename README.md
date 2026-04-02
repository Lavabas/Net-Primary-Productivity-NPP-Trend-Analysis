# Net Primary Productivity (NPP) Trend Analysis Using MODIS & Google Earth Engine - Case Study: India
## Overview
Net Primary Productivity (NPP) is a key indicator of vegetation health, ecosystem productivity, and carbon dynamics. Monitoring its long-term trends helps in understanding climate change impacts, land use changes, and agricultural productivity.

This project analyzes spatiotemporal trends in NPP across India (2001–2024) using MODIS satellite datasets. The workflow integrates Google Earth Engine (GEE) with Python-based tools to extract, process, and statistically analyze vegetation productivity trends over time.

Additionally, the study focuses on cropland areas, enabling targeted insights into agricultural productivity dynamics.

## Objectives
- Analyze long-term NPP trends (2001–2024)
- Focus on cropland-specific productivity patterns
- Detect temporal trends and change points
- Map spatial variability of NPP changes across India

 ## Study Area
- Region: India
- Covers diverse climatic zones including tropical, arid, and temperate regions
- Significant agricultural landscape suitable for productivity analysis

 ## Datasets Used
1. MODIS NPP (MOD17A3HGF)
- Annual Net Primary Productivity
- Unit scaled by 0.0001
- Represents vegetation carbon uptake
2. MODIS Land Cover (MCD12Q1)
- Used to extract cropland areas (Class 12)
- Applied as a mask to isolate agricultural regions

## Tools & Technologies
1. Google Earth Engine (GEE) – Data access and preprocessing
2. Python – Analysis and modeling
3. geemap – Visualization
4. xee – GEE to xarray integration
5. xarray – Multi-dimensional data processing
6. pymannkendall – Trend detection (Mann-Kendall test)
7. pyhomogeneity – Change point detection (Pettitt test)
8. matplotlib – Visualization

## Results Interpretation
### Figure 1: Temporal Trend of Total NPP (2001–2024)
<img width="560" height="432" alt="image" src="https://github.com/user-attachments/assets/d5721c93-1887-43cf-be7c-5c4bda04b439" />

### Figure 2: Spatial Distribution of NPP (2001–2024)
<img width="1723" height="1190" alt="image" src="https://github.com/user-attachments/assets/6d430cf0-5b04-4ed1-b0db-471a07d02ef1" />

### Figure 3: Spatial Trend (Slope) of NPP Change
<img width="587" height="432" alt="image" src="https://github.com/user-attachments/assets/3fc204b0-f0bb-4033-8bed-21fb146e5d2e" />

The temporal analysis of Net Primary Productivity (NPP) across India shows a general increasing trend from 2001 to 2024, with noticeable interannual variability. The time-series plot indicates fluctuations in productivity, with dips around the mid-2010s followed by a strong increase after 2018, reaching peak values in the early 2020s. This suggests a possible improvement in vegetation productivity in recent years, potentially influenced by climatic or agricultural factors.

The spatial maps reveal a clear geographic gradient in NPP distribution. Higher productivity is consistently observed in southern and eastern regions, while northern and northwestern areas (including arid and Himalayan regions) show lower NPP values. Over time, some regions exhibit gradual intensification of productivity, particularly in central and southern India.

The spatial trend (slope) map further highlights regional disparities in change patterns. Large parts of central and western India show positive trends (increasing NPP), indicating improving vegetation or agricultural productivity. In contrast, localized areas, especially in parts of eastern and northeastern regions, display negative or stable trends, suggesting stagnation or potential degradation.

Overall, the results demonstrate that while India shows an overall increase in vegetation productivity, the changes are spatially heterogeneous, reflecting the influence of climate variability, land use practices, and regional environmental conditions.

## Limitations
- MODIS spatial resolution (~500 m–1 km) may not capture field-level variations
- Cropland classification (MCD12Q1) may include misclassification errors
- NPP estimates are model-based, not direct measurements
- Lack of ground validation data for accuracy assessment
- Climate, irrigation, and management practices are not explicitly included

## Notes
1. Cropland masking ensures focused agricultural analysis
2. Xarray enables efficient handling of multi-temporal satellite data
3. The workflow is scalable to other countries or regions
4. Statistical methods enhance reliability of trend detection

