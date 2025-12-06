# E2SFCA
Code to generate geospatial data using the Enhanced Two-step Floating Catchment Area (E2SFCA) method

This repository contains R code that can be used to generate E2SFCA estimates. This code was used to generate estimates of access to surgical care in Ecuador for national planning purposes and for a publication in process. Naming conventions in code are aligned with the healthcare sector, but this code can function for any geospatial analysis using E2SFCA. The code contains the function calculate_e2sfca, which requires a supply dataset (csv file with hospital identifiers and at least 1 supply value such as number of providers), a drivetime dataset (shapefile with hospital identifiers, drivetime distances in seconds, and drivetime polygons), a raster dataset (tif raster file of population counts at the 1kmx1km scale), and a country shapefile (shapefile defining the boundary of the country). Additional arguments are required, such as the supply variables you want to calculate access for, the coordinate system to use for analysis, the value to set for the gaussian decay function, and other naming/filepath related arguments.

In addition to the R code, included is the supply data used for this publication, with hospital names censored. Re-use of the 

Once the publication has been published, a link will be provided in the README. Any use of this code should be cited using the publication citation. The supply data is included for data transparency and reproducibility, and should not be used without express consent of the authors.
