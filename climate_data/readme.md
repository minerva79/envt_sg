# SDOH Asthma Project Data Repository - Mar/Apr 2022

This repository contains datasets scrapped for the Social Determinants of Health (SDOH) Asthma Project conducted in March and April 2022. All data files are stored in the R Data Storage (RDS) format, optimized for use with the R programming language.

## Dataset Overview

### (1) Meta-Data

- **`singapore_v2.rds`**: Dimensions: 131,942 x 5. This dataset includes 6-digit postal codes and their corresponding latitude and longitude coordinates (WGS-84) obtained from OneMap API queries. Postal codes are associated with the 28 postal districts as defined by Singapore postal services, which are further mapped approximately to 5 regions (Central, Northeast, Northwest, Southeast, Southwest) based on postal district descriptions.

- **`planning_area_to_district_code.rds`**: Dimensions: 61 x 2. This file maps the 55 Planning Areas, as utilized in Singapore Household Survey and Census Data, to the 28 Postal Districts used by Singapore postal services.

### (2) Climate Data

- **`nea_historical_13_stations_weather_2015_2021.rds`**: Dimensions: 33,119 x 22. Contains data from 13 weather stations for the period between 2015 and 2021, collated from [NEA's Climate Historical Daily data](http://www.weather.gov.sg/climate-historical-daily/).

- **`noaa_sn_temp_prep.rds`**: Dimensions: 1,988 x 128. Includes scraped NOAA data for temperature and precipitation for one station in Singapore, covering May 1962 to March 2023.

- **`changi_historical_weather_2015_2021.rds`**: Dimensions: 2,557 x 19. Features data from the Changi weather station.

- **`rh2016.rds` to `rh2020.rds`**: XML format; large files. High-frequency (minute-by-minute) relative humidity readings across all weather stations in Singapore, collated from [Data.gov.sg Realtime Weather Readings](https://beta.data.gov.sg/collections/1459/view).

### (3) PSI Data

- **`nea_psi_2016_2020.rds`**: Contains 1,791 lists of up to 24 hourly data rows. Includes readings for pollutants (CO, O3, SO2, NO2, PM2.5, PM10) and the composite index (PSI) for various windows (hourly, four-hourly, eight-hourly, twenty-four-hourly average, and max), sourced from [Data.gov.sg Pollutant Standards Index](https://beta.data.gov.sg/collections/1396/view).
