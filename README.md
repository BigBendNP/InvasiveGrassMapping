## InvasiveGrassMapping

**Exotics_XArray_SatelliteDownload_to_zarr.ipynb** is a notebook that pulls in Landsat data from AWS specific to the Big Bend area and the dates of interest. It also masks the data by grass polygon location.

**Exotics_XArray_Preprocessing.ipynb** converts the Landsat DNs into TOA reflectance values, from which NDVI can be calculated. It also converts the XArray dataset into a Pandas dataframe for ease of analysis.

**Exotics_XArray_NDVI_analysis.ipynb** performs exploratory data analysis (EDA) on the NDVI data for each grass type and compares the data to climatic variables.

**Exotics_XArray_Johnsongrass_Summer.ipynb** pulls in summer NDVI data from Landsat (it also performs the TOA reflectance calculation, so no separate preprocessing notebook is needed) and tries to identify likely Johnsongrass pixels based on NDVI trends from the last week of May to the first week of July. The data can be saved to a GeoTiff for closer examination with ArcGIS or other tools. 
