# Data analysis and forecasting of La Haute Borne wind power data

This set of notebooks goes over the process of importing, analysing and cleaning the open source wind power data from La Haute Borne. The overarching goal is to produce calibrated probabilistic forecasts of the wind power.

## Download the dataset

- Data for 2013-2016 can be downloaded from [Engie](https://opendata-renewables.engie.com/explore/dataset/d543716b-368d-4c53-8fb1-55addbe8d3ad/information). Since the raw dataset is quite large, the reader should download it for themselves. 
- A description of the data features can be downloaded [here](https://opendata-renewables.engie.com/explore/dataset/39490fd2-04a2-4622-9042-ce4dd34c2a58/information).
- The static information, e.g., coordinates or rated power, of the wind farm can be downloaded [here](https://opengie-preprod.ineotinea-gdfsuez.com/explore/dataset/6eeb7f50-97f7-4ab2-8d36-c6d9f9491d84/information).

### Additional features

When forecasting for more than 6 h into the future, it is important to include numerical weather prediction (NWP) forecasts that provide a future estimate of meteorological parameters, sometimes up to 10 days. We'll use forecasts from the Global Forecast System (GFS) maintained by the National Centers for Environmental Prediction because they are open-source and a convenient API is available. These forecasts and features engineered from the raw power measurements will be the inputs to a machine learning model that forecasts the produced power at a certain forecast horizon.

## License

- The GPL v3 License applies to this project, see [LICENSE](https://github.com/DWvanderMeer/LaHauteBorne/blob/main/LICENSE) for more information.
- Note that ENGIE have their own [license](https://www.etalab.gouv.fr/wp-content/uploads/2017/04/ETALAB-Licence-Ouverte-v2.0.pdf) on the dataset as well.

## Acknowledgements

[ENGIE}(https://opendata-renewables.engie.com) is acknowledged for providing such a wealth of useful information online!