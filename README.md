# MODCiX - Mowing Detection Intercomparison Exersice

Grasslands are a major component of Europe's agricultural landscapes and provide important ecological functions and services within a multifunctional agriculture. Grasslands supply fodder, straw or raw biomass for energy production and provide habitat
for endangered flora and fauna. At the same time, there is a wide spectrum of grasslands management practices and intensity, which impact their resilience. Their conservation and sustainable management hence directly contribute to strategies and
policies at the European and national scale aimed at transitioning toward a more sustainable agriculture in the framework of the European Green Deal. Spatially explicit information on the intensity of grassland use is therefore crucial, but mostly
lacking as grassland management practices are usually not reported in agricultural censuses.

Dense time series of remote sensing data were shown to be able to derive information on grassland-use intensity. Several methodological approaches have been published that make use of radar data, optical data, or a combination of both. They either built
on rule-based algorithms relating to underlying biophysical principles or stem from the realm of machine learning techniques. However, most of these studies have a rather local or regional focus, usually being limited by the availability of reference
data they are developed and evaluated from. Tests on model transferability in time - i.e., to different years - and space - i.e., to regions with different environmental conditions and land-use intensities - are usually lacking due to the availabilty of
consistent reference data sets. In addition, different validation strategies inhibit direct comparisons of individual studies. 

To overcome these limitations, we established a network of more than 30 researchers from 8 European countries that brought together a unique reference data set that is representative for several grasslands in Europe with varying climatic and
environmental conditions. The aim of the network is to evaluate existing mowing detection algorithms based on openly accessible satellite data across Europe using a consistent validation framework. The reference data set comprises management information
such as timing or number of mowing events for more than 3,000 grassland parcels covering five years, stretching from Sweden and Estonia in the North to Southern France in the Southwest (see figure). We harmonized the reference data and assigned a certainty label to
each parcel depending on how the information was collected (1: high certainty; e.g., data derived from a webcam to 3: low certainty; e.g., data derived from pixel profile interpretation). For training and calibration requirements, the
reference data are split into training parcels (provided with full information) and validation parcels (only geometries). We pre-processed satellite data from Landsat 7-9, Sentinel-1 and Sentinel-2 for each region and year for which reference data were
available. Based on this data set we run and evaluated a total of currently 8 algorithms that were developed to estimate grassland-use intensity using mowing events as a proxy.

In this repository you will find the codes used to harmonize and clean the reference data, as well as the evaluation codes. The final results will be made available via an R-shiny app once the comparison exercise is finished. Due to data license 
agreements the reference data used will not be openly shared but can be requested through the data owners.


<p align="center">
  <img src="https://github.com/geo-masc/modcix/blob/main/figures/modcix_data_regions.png">
</p>
