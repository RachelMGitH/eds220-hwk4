# Task 2: Visualizing fire scars through false colour

## About:
This repository contains a notebook `hwk4-false-color-MILLER.ipynb` which combines Landsat 8 Satellite data with perimeters of the 2025 Eaton and Palisades fires to create a false colour image visualizing the resulting fire scars.

### Highlights
- Data wrangling and exploration with `xarray` and `geopandas` for geospatial data
- Reprojecting CRS of geospatial data
- Plotting of true-colour and false-colour images
- Creating and customizing a map using three datasets
### About the Data
The data is not housed in this repository. In the notebook two datasets are used:

#### 1.) Landsat Data
This dataset is composed of a simplified collection of bands (red, green, blue, near-infrared and shortwave infrared) from the Landsat Collection 2 Level-2 atmospherically corrected surface reflectance data, collected by the Landsat 8 satellite. This dataset was retrieved from the Microsoft Planetary Computer data catalog and clipped to an area surrounding the fire perimeters. It has been downloaded as a NetCDF file, and contains x and y coordinates, a time stamp, and values for red, green, blue, near infrared and shortwave infrared bands. The data was accessed from a google drive [https://drive.google.com/drive/folders/1USqhiMLyN8GE05B8WJmHabviJGnmAsLP].

#### 2.) Eaton and Palisades Fire Perimeters
This dataset contains fire perimeters for the Eaton and Palisades fires, sourced from CAL FIRE's Historical Fire Perimeter Dataset. Two files were downloaded, one for each fire, as GeoJSON files from [https://egis-lacounty.hub.arcgis.com/maps/ad51845ea5fb4eb483bc2a7c38b2370c/about]. Each file contains one row with 24 columns recording geospatial information on the location of the periemeter and identifying details for the respective fire.  


### References
Center, E. R. O. a. S. (2013). LANDSAT 8-9 Operational Land Imager / Thermal Infrared Sensor Level-2, Collection 2 [Dataset]. In USGS DOI Tool Production Environment. https://doi.org/10.5066/p9ogbgm6 

Palisades and Eaton dissolved fire perimeters (2025). (n.d.). https://egis-lacounty.hub.arcgis.com/maps/ad51845ea5fb4eb483bc2a7c38b2370c/about

## Repository Organization
```
eds220-hwk4
│--  README.md
│--  hwk4-task2-false-color-MILLER.ipynb
│--  .gitignore
```
