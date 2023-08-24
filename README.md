# WECA QGIS file setup guide and release notes
📍 🌐 🌍 📈

Geographical data across the Combined Authority is viewable by staff using 'QGIS' software. A QGIS file exists with various map layers pre-loaded.
To explore our GIS data, follow these steps carefully:
1. Turn on your VPN
2. Navigate to [this folder](https://westofenglandca.sharepoint.com/:f:/r/sites/GIS/Shared%20Documents/General/QGIS_map_file) (open this link in a new tab)
3. Download a copy of the `WECA_GIS_v09.qgz` file into your personal documents. Do not open the file yet.
4. Navigate to where your downloaded file is.
5. Rename the file. Please rename the copied file by adding your name and surname initial to the end (eg. `WECA_GIS_v09_TheoF.qgz`).
6. Open the file. Please allow **2-3 minutes** or so for QGIS to fully load the layers (there are lots of map layers!). Try not to interact with QGIS during loading.

Release notes are available below for the latest QGIS `.qgz` file. A new release of this file is expected every couple of months. Check the folder linked above for updated versions, then repeat the steps above if `v10` is found.

---

📚🎥 Training docs and videos can be found [here](https://westofenglandca.sharepoint.com/:f:/r/sites/GIS/Shared%20Documents/General/Training).

📔📑 The GIS data catalogue can be found [here](https://westofenglandca.sharepoint.com/:x:/r/sites/GIS/_layouts/15/Doc.aspx?sourcedoc=%7BCF113E21-93A4-42AC-AEFF-26530EF1A1D6%7D&file=WECA_GIS_data_catalogue.xlsx&action=default&mobileredirect=true). (constantly updated)

---

## **QGIS file (.qgz) release history:**

## **Version 09** (June 2023)

###### New
* previous month's release of SWPTI/National PTI bus data added (change also appears in v08 as of 22/12/22)
* update log table for SWPTI/National PTI bus data added (change also appears in v08 as of 22/12/22)
* integrated micromobility service (IMS) areas
* BRERC habitat map (change also appears in v08 as of 09/01/23)
* CRSTS/TCF W&C scheme overhaul/update
* update log table for all regularly updated datasets
* cycle hangars
* DRT WESTlink zones (March 2023)
* cycling and walking routes (JLTP4 & LCWIP)
* car club bays (Travelwest)
* combined active + inactive bus stops
* LCWIP and JLTP4 cycling routes
* historical tramways
* cities and towns name labels
* A2 landscape technical drawing template added to layouts
* 'DRAFT' watermark added to each layout
* WoE+ Zone shape added to First Bus fare zone layer
* DfT/OS strategic road network
* OS building height data
* BCC owned land
* Job Centre locations
* Bee Bold award winners and shortlisters (2022 & 2023 layers)

###### Changed
* 'SWPTI' layer group renamed to 'National PTI (SWPTI/Traveline)'
* 'Previous month's release' changed to 'Previous release' for SWPTI data (due to potential of skipped months)
* National PTI monthly data update now working again, after Feb-May issues with data supply
* National PTI monthly data now contains WESTlink services (with new symbology)
* set scale dependent visibility on 'Land parcels' layer
* all A3 & A4 Layout templates set to 200dpi export resolution and 'Print as raster' by default
* all Layout templates have 'Only show items inside linked map' unchecked by default (can reduce Layout opening time)
* 'E-scooters' layer group renamed to 'Micromobility'

###### Removed
* SWPTI ptways_y10/plus and pylinks_y10/plus layers (these appeared to be duplicates of the SWPTI 'Bus routes' layer)
* OS MasterMap greenspace (seems superfluous)

###### Issues
* slow initial project file loading time (approx. 2-3 minutes). There is an official scheduled [fix](https://github.com/qgis/QGIS/pull/53112) for this issue in QGIS software update (v3.32.0), available on 26th June. Testing outcomes to be shared on GIS Teams group chat nearer the time. If successful, new QGIS software will be auto-installed on user laptops, replacing current QGIS software v3.22.8.

## **Version 08** (November 2022)

###### New
* first iteration of QGIS file with new layout
* layers now hosted in Azure cloud, on PostgreSQL databases
* multiple new layers added - see data catalogue for full list

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

## **Version 10** (TBC Q3 2023)

###### New
* MetroBus stops and routes
* Think Broadband dataset (July 2023 update)
* Clean Air Zone (CAZ) for Bath and Bristol

###### Changed

###### Removed

###### Planned
* BCC Adopted Highways
* add SW rail lines
* add destination data (employment centres, schools etc.)
* Google Street View bus stop layer
* travel to work data
* carbon data, carbon.place (data added 14/06/23 as creds.pbcc_lsoa_lep, but due to number of columns in dataset, risk of project slowdown until QGIS 3.32.0 software release)
* flood projection polygons, if not RoFRS or RoFSW existing datasets
