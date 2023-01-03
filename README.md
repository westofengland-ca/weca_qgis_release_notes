# WECA QGIS file release notes
📍 🌐 🌍 📈

Geographical data across the Combined Authority is viewable by staff using 'QGIS' software. A QGIS file exists with various map layers pre-loaded.
To explore our GIS data, follow these steps:
1. Turn on your VPN
2. Navigate to [this folder](https://westofenglandca.sharepoint.com/:f:/r/sites/GIS/Shared%20Documents/General/QGIS_map_file)
3. Download a copy of the `WECA_GIS_v08.qgz` file into your personal documents. Do not open the file yet.
4. Navigate to where your downloaded file is.
5. Rename the file. Please rename the copied file by adding your name and surname initial to the end (eg. `WECA_GIS_v08_TheoF.qgz`).
6. Open the file. Please allow **2 minutes** or so for QGIS to fully load the layers (there are lots of map layers!). Try not to interact with QGIS during loading.

Release notes are available below for the latest QGIS `.qgz` file. New releases are expected every couple of months. Check the folder linked above for updated versions.

---

📚🎥 Training docs and videos can be found [here](https://westofenglandca.sharepoint.com/:f:/r/sites/GIS/Shared%20Documents/General/Training).

👥🎥 GIS catchup recording demos can be found [here](https://westofenglandca.sharepoint.com/:f:/r/sites/GIS/Shared%20Documents/General/Catch-ups/Recordings).

📔📑 The GIS data catalogue can be found [here](https://westofenglandca.sharepoint.com/:x:/r/sites/GIS/_layouts/15/Doc.aspx?sourcedoc=%7BCF113E21-93A4-42AC-AEFF-26530EF1A1D6%7D&file=WECA_GIS_data_catalogue.xlsx&action=default&mobileredirect=true) (WIP).

---

## **QGIS file (.qgz) release history:**

## **Version 08** (November 2022)

###### New
* first iteration of QGIS file with new layout
* layers now hosted in Azure cloud, on PostgreSQL databases
* multiple new layers added - see data catalogue for full list.


###### Changed
* layer rendering performance after switch to Azure cloud data sources


###### Removed
* GIS file server datasets removed as data sources


###### Issues
* slow initial project file loading time (1.5-2 minutes)
* slow map layer load on first layer chosen

## **Versions 01-07** (September 2021-October 2022)
###### Summary
* QGIS map file reading Shapefile data from Agilisys file server
* each update added more map layers


###### Issues
* slow read/write performance
* slow map rendering performance
* file based data - non-relational & inefficient
* limited bandwidth and scalability
* externally managed

---
---
---

## **QGIS file (.qgz) release future schedule:**

## **Version 09** (TBC Q2 2023)

###### New
* previous month's release of SWPTI/National PTI bus data added (change also appears in v08 as of 22/12)
* update log table for SWPTI/National PTI bus data added (change also appears in v08 as of 22/12)

###### Changed
* 'SWPTI' layer group renamed to 'National PTI (SWPTI)'
* set scale dependent visibility on 'Land parcels' layer
* all Layout templates set to 200dpi export resolution and 'Print as raster' by default
* all Layout templates have 'Only show items inside linked map' unchecked by default (can reduce Layout opening time)

###### Removed
* SWPTI ptways_y10/plus and pylinks_y10/plus layers (these appeared to be duplicates of the SWPTI 'Bus routes' layer)

###### Issues
* slow initial project file loading time (approx. 2 minutes)

###### Planned
* add more print template options to the Layout Manager
* add cycle hangars dataset
* add WoE+ Zone shape to First Bus fare zone layer
