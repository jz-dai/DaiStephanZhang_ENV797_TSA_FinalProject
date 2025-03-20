# DaiStephanZhang_ENV797_TSA_FinalProject

R code and datasets for the final project of ENV797 Spring 2025 for J. Dai, R. Stephan, and Z. Zhang.

# Summary

# Investigators

-   Jingze Dai, Duke University Nicholas School of the Environment,
    [jd559\@duke.edu](mailto:jd559@duke.edu),
    contributor

-   Rachael Stephan, Duke University Nicholas School of the Environment,
    [rachael.stephan\@duke.edu](mailto:rachael.stephan@duke.edu),
    contributor

-   Zuocheng Zhang, Duke Kunshan University,
    [zz352\@duke.edu](mailto:zz352@duke.edu),
    contributor

    
# Keywords

#climatechange, #greenhousegases, #GHG, #methane, #NOAA, #airquality

# Database Information

Globally averaged methane data used in this analysis was retrieved from [NOAA's page on greenhouse gas trends](https://gml.noaa.gov/ccgg/trends_ch4/). This global averages were obtained by curve fitting and smoothing data from well-mixed marine boundary layer (MBL) air. MBL air is considered representative of the larger atmosphere. More details on this process can be found at [this webpage](https://gml.noaa.gov/ccgg/about/global_means.html).

For this analysis, the contributors:

1.  Wrangled and subset the global averages into training and test data sets.

2.  

# Folder & Data Structure and Naming Conventions

## Folder Structure

The primary folders in the repository are `Data` and `Code`.

-   `Code` contains all of the R code associated with the timeseries analysis.

-   `Data` contains all of the data for the analysis. It contains the following
    sub-folders

    -   `Data/Raw`: all of the raw data sets.

    -   `Data/Processed`: all of the processed data in a format that is easily readable in R

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

-   Wrangling_Visualization: Contains the upload and basic wrangling of monthly data, subsetting into training and test data, and an initial visualization of the entire dataset.
