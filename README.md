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
🛠️ Steps Performed
1. Buffer Analysis
Tool used: Buffer (Analysis Tools → Proximity → Buffer)

Input: Johnson (facility point data)

Distance: 500 meters

Output: Johnson_Buffer

2. Spatial Join
Tool used: Spatial Join (Analysis Tools → Overlay → Spatial Join)

Target Feature: Sensitive_Receptors

Join Feature: Johnson_Buffer

Match Option: INTERSECT

Output: Sensitive_Recept_SpatialJoin

Result: Identified which sensitive features (schools, hospitals) are within buffer zones of contaminant sources.

3. Map Layout and Visualization
Labels added for major facilities and parks.

Categories styled using Facility_T field.

Layout exported to Contaminant_Soure_Layout.png.
📊 Outputs
Sensitive_Recept_SpatialJoin layer with joined attributes.

Contaminant_Soure_Layout.png map layout for presentation.

Join_Count attribute indicates number of overlapping buffer zones.


