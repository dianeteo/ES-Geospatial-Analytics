# Codes for extracting geospatial data from NASA's Landsat images for the purposes of investigating various phenomena

For my project under the Ministry of Trade & Industry's Economist Service (ES) Internship programme, I leveraged data from Google Earth Engine, Open Street Map (OSM) and GeoSpace (GS) to investigate the effectiveness of heat mitigation policies on behalf of the Ministry of Sustainability and Environment in Singapore with econometric modelling. In this project, we look at:
1. The effect of greenery on Land Surface Temperatures (LST), where greenery is measured by NDVI;
  a. The clearing of land for the construction of BTO flats in Singapore;
  b. HDB's mandatory Green Plot Ratio of 4.5 for all HDB developments from the year 2016 onwards
2. The effect of solar panel installations on industrial buildings and HDB flats in Singapore;
3. The effect of cool paints in HDB towns, industrial areas and hawker centres in Singapore using a Differences-in-Differences method

# Code breakdown
1. In `Landsat Codes > 1_Download_Landsat_Images`, codes can be run to download specific Landsat scenes from specified collections and to convert images into tabular format (where each 30 by 30 metre pixel represents a single row of data)
2. In `Landsat Codes > 2_Heatmaps`, codes can be run to plot LST of Singapore using different packages (hvPlot provides the best visualisation)
3. In `Landsat Codes > 4_Extracting_Pixels`, codes can be run to extract pixels of specific regions of interest by combining Geospatial data from OSM and GS with band-specific information
4. In `Landsat Codes > 4_DiD_Regression`, codes can be run to conduct DiD regression for specific cool-painted (treated) areas; pre-trends test and dynamic effects model have also been conducted to check for parallel trends and long-term effects
5. In `Landsat Codes > 5_Descriptive_Statistics`, codes can be run to identify longitudinal and cross-sectional relationships between LST and NDVI across HDB towns in Singapore, as well as looking into the effectiveness of solar panel installations and greenery in reducing LST
6. In `Ambient Temperatures`, codes can be run to identify the best predictors of the relationship between LST and ambient temperatures (air temperatures) recorded by weather stations in Singapore
