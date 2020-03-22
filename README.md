# WRF-Topographic-Plots-Including-Nested-Domains-Example
Python code that plots topographic data as individual layers onto one figure from pre-processed wrfout*.nc files. 

Example Python code that,
1) Plots WRF topographic data for multiple domains using "pcolormesh" (a single wrfout file [for each domain] has been pre-processed into gridded NETCDF files using the 'NOAA Weather and Climate Toolkit'). For windows' users, processing an entire .nc file from WRF will likely crash your PC. It's better to post-process the 'HGT' field from a single .nc file from WRF, then import it into Python.
2) Plots each individual domain boundary (from pre-processed wrfout*.nc files via ArcMap using the "aggregate by points" tool). This can be done using Python... Will add in the future if applicable.
3) Plots stations within the domain (pre-processed wrfout*.nc files via ArcMap using the "select by location tool"). Likewise, this can be done using Python...

Required input: 
wrfout*.nc (or met_em*.nc) file(s)

Output:
pdf/png of WRF's domain

Required libraries include,
pandas 
numpy
matplotlib
netCDF4

Recommended Pre-processing tool,
NOAA Weather and Climate Toolkit (free software): https://www.ncdc.noaa.gov/wct/ for 'HGT' extraction from wrfout*.nc file(s). Will crash your PC otherwise...

Optional Pre-processing tools,
ArcMapv10.2 (private) or in all likliehood (haven't tried), QGIS (free) for shapefile/boundary lines & station identification.

Future,
Optional pre-processing tools aren't required and can be done using Python... Will add in the future if need be or requested.
