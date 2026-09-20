# GIS-Based Flood Risk Analysis of Lagos State, Nigeria

## Project Overview

This project presents a GIS-based spatial analysis of potential flood exposure across Local Government Areas (LGAs) in Lagos State, Nigeria.

The analysis uses **waterway proximity** as a spatial indicator of potential flood risk. A **500-metre buffer** was created around waterways, and the buffer was intersected with Lagos State LGAs to determine the proportion of each LGA located within 500 metres of a waterway.

The analysis was carried out using **QGIS** and projected coordinate data suitable for distance and area calculations.

## Objectives

* Identify Lagos LGAs located within 500 metres of waterways.
* Calculate the area of each LGA within the 500-metre waterway buffer.
* Calculate the percentage of each LGA located within the buffer.
* Visualize the spatial distribution of waterway proximity across Lagos State.
* Demonstrate how GIS can support flood-risk assessment and spatial planning.

## Methodology

The workflow consisted of the following major steps:

1. Prepared the Lagos State LGA boundary data.
2. Prepared the waterway data.
3. Created a **500 m buffer** around waterways.
4. Reprojected the data to **EPSG:32631 (WGS 84 / UTM zone 31N)** for metric distance and area calculations.
5. Intersected the LGA boundaries with the waterway buffer.
6. Calculated the area of intersected regions.
7. Summarized the buffered area by LGA.
8. Calculated the percentage of each LGA within the 500 m buffer.
9. Created a graduated thematic map showing the results.

## Key Output

The final map visualizes the percentage of each Lagos LGA that falls within 500 metres of waterways.

Higher percentages indicate a greater proportion of an LGA located within the defined waterway-proximity zone. This provides a spatial indicator that can be used alongside other environmental, topographic, drainage, rainfall, and socioeconomic factors in a broader flood-risk assessment.

## Project Structure

```text
Lagos-flood-risk-analysis/
│
├── data/
│   └── Input GIS datasets
│
├── maps/
│   └── Lagos LGA Waterway Map.pdf
│
├── outputs/
│   ├── Lagos_LGAs_Final_32631.shp
│   ├── Lagos_LGAs_Final_32631.shx
│   ├── Lagos_LGAs_Final_32631.dbf
│   ├── Lagos_LGAs_Final_32631.prj
│   └── Lagos_LGAs_Final_32631.cpg
│
└── README.md
```

## Software

* QGIS
* GIS vector processing tools
* Spatial overlay and buffer analysis

## Coordinate Reference System

**EPSG:32631 — WGS 84 / UTM Zone 31N**

This projected coordinate reference system was used to support distance and area calculations in metres.

## Disclaimer

Waterway proximity is used in this project as an indicator for spatial flood-risk analysis. Proximity to a waterway does not by itself determine whether an area will flood. A comprehensive flood-risk assessment would also consider factors such as elevation, drainage capacity, rainfall, land use, soil characteristics, historical flood events, and exposure and vulnerability.

## Author

GIS-Based Flood Risk Analysis Project

---

*This project demonstrates the application of GIS and spatial analysis techniques to an environmental risk assessment problem in Lagos State, Nigeria.*## Final Map

The map below shows the percentage of each Lagos State LGA located within 500 metres of waterways.

![Lagos LGA Waterway 500m Percentage Map](../maps/Lagos_LGA_Waterway_500m_Percentage_Map.png)

