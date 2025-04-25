# DaiStephanZhang_ENV797_TSA_FinalProject

R code and datasets for the final project of ENV797 Spring 2025 for J. Dai, R. Stephan, and Z. Zhang.

# Summary

This repository serves as container for data and analysis used in an forecasting analysis of global methane concentrations and temperature anomalies. Methane is a greenhouse gas (GHG), and it's anthropogenically increased concentrations in the atmosphere have play a part in Earth's increased heat budget. The investigators connected methane concentrations to beef production and socioeconomic factors. The research initiative was inspired by the high importance methane has on short-term (decades) climate. The data was collected by NOAA, USDA, and the Federal Reserve Bank of Dallas.

Our analysis aims to:

1.  Forecast methane concentrations with multiple different forecast models, using beef production and socioeconomic factors as predictors, to identify the most accurate model for short-term forecasting.

2.  Forecast temperature anomalies using historical and forecasted methane concentrations to identify a future climate scenario, assuming operations remain as-is.

The repository contains all raw and wrangled data sets, visualizations, analysis, and associated R code used to answer the above research questions.

# Investigators

-   Jingze Dai, Duke University Nicholas School of the Environment,
    [jd559\@duke.edu](mailto:jd559@duke.edu),
    contributor

-   Rachael Stephan, Duke University Nicholas School of the Environment,
    [rachael.stephan\@duke.edu](mailto:rachael.stephan@duke.edu),
    contributor

-   Zuocheng Zhang, Duke University Nicholas School of the Environment,
    [zz352\@duke.edu](mailto:zz352@duke.edu),
    contributor

    
# Keywords

#climatechange, #greenhousegases, #GHG, #methane, #NOAA, #airquality

# Database Information

Globally averaged methane data used in this analysis was retrieved from [NOAA's page on greenhouse gas trends](https://gml.noaa.gov/ccgg/trends_ch4/) run by the NOAA Global Monitoring Laboratory. This global averages were obtained by curve fitting and smoothing data from well-mixed marine boundary layer (MBL) air. MBL air is considered representative of the larger atmosphere. More details on this process can be found at [this webpage](https://gml.noaa.gov/ccgg/about/global_means.html). 

Global temperature anomaly data was retrieved from the [NOAA National Center for Environmental Information](https://www.ncei.noaa.gov/access/monitoring/climate-at-a-glance/global/time-series). The global average temperature anomaly was calculated using a climate baseline averaged over 1901-2000. The data set has a spatial coverage over the [land](https://www.ncei.noaa.gov/products/land-based-station/global-historical-climatology-network-monthly) and [ocean](https://www.ncei.noaa.gov/products/extended-reconstructed-sst) that has been combined into a single data product.

Beef production data was gathered from the U.S. Department of Agriculture. It is an aggregated worldwide beef production metric. 

Socioeconomic factors data were retrieved from the Federal Reserve Bank of Dallas. 

For this analysis, the contributors:

1.  Wrangled and subset all the raw data sets into training and test data sets.

2.  Trained various models on the training data to produce a forecast

3.  Analysed the accuracy / performance metrics of each forecast to identify the best models.

# Folder & Data Structure and Naming Conventions

## Folder Structure

The primary folders in the repository are `Data`, `Figures`, and `Code`.

-   `Code` contains all of the R code associated with the timeseries analysis.

-   `Data` contains all of the data for the analysis. It contains the following
    sub-folders:

    -   `Data/Raw`: all of the raw data sets.

    -   `Data/Processed`: all of the processed data in a format that is easily readable in R
    
-   `Forecasts` contains all of the forecasts and top accuracy statistics produced held in `.csv` files. It contains the following sub-folders:

    -   `Forecasts/Methane`: all of the forecasts for methane concentrations
    
    -   `Forecasts/Temperature`: all of the forecasts for temperature anomalies
    
The `Progress_Tracker.txt` was only contained within the project and not any folders. This file was the task organizer for the project.

This `README.md` file was only contained within the project and not any folders.

## File Formats

-   The project was created with a `.Rproj` file

-   The read me is saved as a `.md` file

-   All raw data frames were uploaded as `.csv` files.

-   All processed data frames were saved as `.csv` files.

-   All R code was written in `.rmd` files.

-   The final report was knitted into a `.pdf` file.

# Metadata

# Scripts and Code

All R code is contained in Rmarkdown documents location in the `Code`
folder.

-   Wrangling: Contains the upload and basic wrangling of monthly data, subsetting into training and test data, and an initial visualization of the entire dataset.

-   Rachael_Methane_Forecasting: Contains all of the methane forecasts conducted using solely methane concentration data conducted by Rachael with some code from Zhuocheng and Jingze included.

-   Rachael_Temperature_Forecasting: Contains all of the temperature forecasts conducted using methane concentration data as a predictor for temperature conducted by Rachael.

-   Forecast_Averaging: Contains all of the code that will process all produced forecasts and calculate the average forecasts of every combination and their performance statistics.

-   Final_Project: Contains all of the most relevant output from all of the above scripts and the analysis write-up.
