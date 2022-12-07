# WECA QGIS file release notes
📍 🌐 🌍 📈

Geographical data across the Combined Authority is viewable by staff using 'QGIS' software. A QGIS file exists with various map layers pre-loaded.
To explore our GIS data, navigate to [this folder](https://westofenglandca.sharepoint.com/:f:/r/sites/GIS/Shared%20Documents/General/QGIS_map_file), then ***download a copy of the `.qgz` file into your personal documents and rename the file***. Please rename the copied file by adding your name and surname initial to the end (eg. `WECA_GIS_v08_TheoF.qgz`). When opening the file, please allow **2 minutes** for QGIS to fully load the layers.

Release notes are available below for the latest QGIS `.qgz` file. New releases expected every couple of months. Check the folder linked above for updated versions.

Training material can be found [here](https://westofenglandca.sharepoint.com/:f:/r/sites/GIS/Shared%20Documents/General/Training).
GIS catchup recording demos can be found [here](https://westofenglandca.sharepoint.com/:f:/r/sites/GIS/Shared%20Documents/General/Catch-ups/Recordings). The GIS data catalogue can be found [here](https://westofenglandca.sharepoint.com/:x:/r/sites/GIS/_layouts/15/Doc.aspx?sourcedoc=%7BCF113E21-93A4-42AC-AEFF-26530EF1A1D6%7D&file=WECA_GIS_data_catalogue.xlsx&action=default&mobileredirect=true) (WIP).

## **QGIS file (.qgz) release history:**

## **Version 08** (November 2022)

###### New
* first iteration of QGIS file with new layout
* layers now hosted in Azure cloud, on PostgreSQL databases
* multiple new layers added - see data catalogue for full list.


###### Improved
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
