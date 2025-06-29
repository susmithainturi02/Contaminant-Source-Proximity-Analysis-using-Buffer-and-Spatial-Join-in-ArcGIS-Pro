# Contaminant-Source-Proximity-Analysis-using-Buffer-and-Spatial-Join-in-ArcGIS-Pro
This GIS project identifies sensitive receptors that are within proximity to contaminant sources by performing Buffer Analysis and Spatial Join in ArcGIS Pro. The workflow demonstrates how to generate buffer zones around identified facilities and spatially analyze which sensitive locations fall within those zones to support risk assessment.
# 🛰️ Contaminant Source Proximity Analysis using ArcGIS Pro

This project performs a proximity analysis using **Buffer** and **Spatial Join** tools in **ArcGIS Pro** to identify **sensitive receptors** (such as schools, hospitals, and parks) that may be impacted by nearby **contaminant sources**. The result supports decision-making for environmental risk assessments and urban planning.

---

## 📌 Objective

To determine which sensitive locations fall within a specified buffer zone (500 meters) around potential contaminant sources and visualize the results in a clear layout map.

---

## 🗂️ Folder Structure

```bash
Contaminant-Source-Buffer-Analysis/
│
├── data/
│   ├── sensitive_receptors.shp
│   ├── contaminant_sources.shp
│   └── Johnson_Buffer.shp
│
├── maps/
│   ├── Contaminant_Soure_Buffer_Analysis.png
│   └── Contaminant_Soure_Layout.png
│
├── scripts/
│   └── spatial_analysis_script.py
│
└── README.md
