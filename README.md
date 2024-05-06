# Madrid Dataset
Dataset submitted to the International Journal of Geographical Information Science for review, as part of the paper "Smart Beestricts: Improving the Spatial Resolution of Air-Quality Data in Madrid through Transfer Learning". Author information hidden for double-blind review.

The data is presented in three formats: **raw data** presents the original raw data mapped to station locations according to the data source, **processed data** includes temporal data interpolation and removal of frozen stations, and **aggregated data** presents the data aggregated to H3 grid using a resolution of 7. All the data is available in .pkl format based on GeoPandas Dataframes.

Acknowledgement for original data [[1](https://datos.madrid.es/portal/site/egob)], [[2]((http://www.emtmadrid.es))]: "Origen de los datos: Ayuntamiento de Madrid" / "Powered by EMT de Madrid".

### Folder structure
```
.
├── air_pollution
|   ├── raw_data               # GeoPandas DataFrame of raw data (mapped to station location)  
|   |   ├── gdf_CO.pkl
|   |   ├── gdf_NO2.pkl
|   |   ├── gdf_O3.pkl
|   |   ├── gdf_PM10.pkl
|   |   ├── gdf_PM2.5.pkl
|   |   └── gdf_SO2.pkl
|   ├── processed_data         # GeoPandas DataFrame of processed data (filtered and re-sampled) 
|   |   ├── gdf_CO.pkl
|   |   ├── gdf_NO2.pkl
|   |   ├── gdf_O3.pkl
|   |   ├── gdf_PM10.pkl
|   |   ├── gdf_PM2.5.pkl
|   |   └── gdf_SO2.pkl
|   ├── aggregated_data        # GeoPandas DataFrame of hexagon-aggregated data 
|   |   ├── gdf_CO.pkl
|   |   ├── gdf_NO2.pkl
|   |   ├── gdf_O3.pkl
|   |   ├── gdf_PM10.pkl
|   |   ├── gdf_PM2.5.pkl
|   |   └── gdf_SO2.pkl
├── traffic
|   ├── raw_data               # GeoPandas DataFrame of raw data (mapped to station location)  
|   |   └── gdf_traffic.pkl
|   ├── processed_data         # GeoPandas DataFrame of processed data (filtered and re-sampled) 
|   |   └── gdf_traffic.pkl
|   ├── aggregated_data        # GeoPandas DataFrame of hexagon-aggregated data 
|   |   └── gdf_traffic.pkl
├── weather
|   ├── raw_data               # GeoPandas DataFrame of raw data (mapped to station location)  
|   |   ├── gdf_temperature.pkl
|   |   ├── gdf_relhumidiy.pkl
|   |   └── gdf_irradiation.pkl
|   ├── processed_data         # GeoPandas DataFrame of processed data (filtered and re-sampled)  
|   |   ├── gdf_temperature.pkl
|   |   ├── gdf_relhumidiy.pkl
|   |   └── gdf_irradiation.pkl
|   ├── aggregated_data        # GeoPandas DataFrame of hexagon-aggregated data 
|   |   ├── gdf_temperature.pkl
|   |   ├── gdf_relhumidity.pkl
|   |   └── gdf_irradiation.pkl
└── meteorology	
    ├── raw_data               # GeoPandas DataFrame of raw data (mapped to station location) 
    |   ├── gdf_wind.pkl
    |   ├── gdf_barometric_pressure.pkl
    |   └── gdf_rain.pkl
    ├── processed_data         # GeoPandas DataFrame of processed data (filtered and re-sampled) 
    |   ├── gdf_wind.pkl
    |   ├── gdf_barometric_pressure.pkl
    |   └── gdf_rain.pkl
    └── aggregated_data        # GeoPandas DataFrame of hexagon-aggregated data
        ├── gdf_wind.pkl
        ├── gdf_barometric_pressure.pkl
        └── gdf_rain.pkl
```
