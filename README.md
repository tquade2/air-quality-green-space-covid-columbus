# Green Space, Air Quality, and COVID Cases in Columbus, OH

This repository contains code for mapping and analyzing green space, air quality, and COVID cases in Columbus, OH. The code utilizes various R packages, including `sf`, `tidyverse`, `tmap`, `tidycensus`, `tigris`, `rgeos`, `rgdal`, `raster`, `exactextractr`, `corrplot`, and `rmapshaper`.

The code first downloads zip code data from the American Community Survey (ACS) using the `tidycensus` package, calculates the percent race/ethnicity and median income for each zip code, and clips the zip codes to the Columbus city boundary using the `sf` package. The code then reads air quality data and landsat data, and calculates the Normalized Difference Vegetation Index (NDVI) for each zip code. It also reads COVID case data and joins it with the zip code data. Finally, the code creates maps using `tmap`, and generates a correlation matrix and scatterplots to analyze the relationships between green space, air quality, and COVID cases with the percent of the population that is black.

## Getting Started

To run this code, you will need to have R and the necessary packages installed. You will also need to have an API key for the Census Bureau API.

1. Install R from the [R Project website](https://www.r-project.org/).
2. Install the required packages using the following command: `install.packages(c("sf", "tidyverse", "tmap", "tidycensus", "tigris", "rgeos", "rgdal", "raster", "exactextractr", "corrplot", "rmapshaper", "ncdf4"))`
3. Obtain an API key for the Census Bureau API by following the instructions [here](https://api.census.gov/data/key_signup.html).
4. Set the working directory to the location of the code and data files.
5. Replace `YOUR DIRECTORY HERE` and `YOUR API KEY HERE` with your directory path and API key in the code.

## Running the Code

To run the code, open the R file and run each line of code in sequence.

The code will generate the following:

- A map of the clipped zip codes
- A map of air quality data
- A map of NDVI
- A map of COVID cases per 100k people
- A map of green space
- A correlation matrix of the variables
- Scatterplots of green space, air quality, and COVID cases with the percent of the population that is black

## Data Sources

- American Community Survey (ACS) from the Census Bureau API
- Air quality data from the National Centers for Environmental Information (NCEI)
- Landsat data from the US Geological Survey (USGS)
- COVID case data from the Columbus Department of Public Health

## Authors

This code was written by Taylor Quade.

## License

This project is licensed under the MIT License - see the `LICENSE` file for details.
