# WECA QGIS file release notes
📍 🌐 🌍 📈

Release notes for the main WECA QGIS .qgz file, located in folder: `\\gismap\GIS\Server_database\WECA_QGIS_main`

## **Version 08** (November 2022)

###### New
* first iteration of QGIS file with new layout
* layers now hosted in Azure cloud, on PostgreSQL databases
* multiple new layers added - see data catalogue for full list: [WECA GIS data catagloue](https://westofenglandca.sharepoint.com/:x:/r/sites/GIS/_layouts/15/Doc.aspx?sourcedoc=%7BCF113E21-93A4-42AC-AEFF-26530EF1A1D6%7D&file=WECA_GIS_data_catalogue.xlsx&action=default&mobileredirect=true)
###### Improved
* layer rendering performance after switch to Azure cloud data sources
###### Removed
* GIS file server datasets removed as data sources

## **Versions 01-08** (June 2021-October 2022)
###### Summary
* QGIS map file reading Shapefile data from Agilisys file server
###### Issues
* slow read/write performance
* slow map rendering performance
* file based data - non-relational & inefficient
* limited bandwidth and scalability
* externally managed
