Files here are data scrapped for the SDOH Asthma Project in Mar/Apr 2022. All files are in RDS (R Data Storage) format, a file format used in R.

(1) Meta-Data
- singapore_v2.rds: (dim. 131942 x 5) Consist of 6 digit postal code and the corresponding latitude-longitude (WGS-84) based on OneMap API query. Postal codes are mapped to the 28 districts (postal districts as defined by Singapore postal services). Districts are approximately mapped to the 5 regions (central, northeast, northwest, southeast, southwest) based on the description of the postal districts.
- planning_area_to_district_code.rds: (dim. 61 x 2) Mapping of the 55 Planning Area (as used in Singapore Household Survey and Census Data) to the 28 Postal Districts (as used in Singapore postal services)


(2) Climate-Data
- nea_historical_13_stations_weather_2015_2021.rds: (dim. 33119 x 22) Consist of 13 Weather stations for period between 2015 and 2021. Data collated from http://www.weather.gov.sg/climate-historical-daily/
- noaa_sn_temp_prep.rds: (dim. 1988 x 128) Consist of scraped NOAA data for temperature and precipitation for one station in Singapore from May 1962 to March 2023.
- changi_historical_weather_2015_2021.rds: (dim. 2557 x 19) Consist of Changi weather station data.
- rh2016.rds to rh2020.rds: (XML format; large) High frequency (minute reading) of relative humidity across all weather station in Singapore. Data collate from Data.gov.sg Realtime Weather Readings (https://beta.data.gov.sg/collections/1459/view) 
