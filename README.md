# BDA602_MachineLearning
Abstract 

Like most global industries, the COVID-19 pandemic caused fundamental shifts in the airline industry.  As a result, the consumer is often left with the inconvenience of delayed and canceled flights for various reasons. In this project, we explored a large dataset of canceled and delayed flights from 2019-2023 from the US from the Department of Transportation along with weather data from NOAA, leveraged machine learning models to identify trends in delayed and canceled flights, and created a tool that consumers can use to predict the probability that their upcoming flight will be delayed or canceled. After using several machine learning models, we utilized an Extreme Gradient Boosting (XGBoost) that achieved an accuracy of 0.68 and a weighted average f1-score of 0.70.

About the Datasets
Flight Delay and Cancellation Dataset (2019-2023): 
Our primary dataset originates from the U.S. Department of Transportation, specifically sourced from the Bureau of Transportation Statistics, spanning the years 2019 to 2023. This comprehensive dataset, available via Kaggle, encompasses a vast array of flight-related information, comprising 32 attributes and a staggering 3 million rows. Among its contents are detailed flight routes denoting origin and destination points, event durations, as well as insights into the reasons behind flight delays and cancellations. 
(https://www.kaggle.com/datasets/patrickzel/flight-delay-and-cancellation-dataset-2019-2023/data)
Weather Dataset: 
To enrich our analysis, we incorporated weather data sourced from the National Oceanic and Atmospheric Administration (NOAA). This dataset is called the Daily Global Historical Climatology Network (GHCN-Daily) and is available through their website.  It provides a wealth of meteorological information essential for contextualizing flight operations within the United States. This data is a collection of many different daily measurements for stations across the globe, and many of these stations are located at or very close to airports. The five core elements of this data describe precipitation, snowfall, snow depth, maximum temperature, and minimum temperature. The additional measurement of average daily wind speed was included in this project because it is an essential consideration for pilots. Precipitation is in tenths of a mm, snow measurement is in mm and temperature is in tenths of a degree Celsius. Wind speed is measured in mm per second.
https://www.ncei.noaa.gov/access/metadata/landing-page/bin/iso?id=gov.noaa.ncdc:C00861
(https://noaa-ghcn-pds.s3.amazonaws.com/index.html)
Coordinates for Airports Dataset:
To bridge the gap between the flight and weather datasets, we used the International Air Transport Association/International Civil Aviation Organization (IATA/ICAO) list data from http://www.ip2location.com. This data set includes the country code, region name, IATA code, and ICAO code. airport name, latitude, and longitude. The International Air Transport Association (IATA) code was used to merge the code on the flight data to assign geographic markers to each airport in our flight dataset. 

(https://github.com/ip2location/ip2location-iata-icao/blob/master/iata-icao.csv)

