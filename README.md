# failure_warning
Time-stamped data used for the case study of the developed failure warning system.
They relate to HVDC line Konti-Skan (power line between Sweden and Denmark).

## Description of data and sources

* Maintenance: planned maintenance activity at the line, expressed as a binary variable (0: maintenance activity did not occur and 1: maintenance activity occurred) and non-binary variable (counting the number of steps between 2 maintenance activities).
* Failure: unplanned maintenance activity at the line, expressed as a binary variable (0: failure did not occur and 1: failure occurred) and non-binary variable (counting the number of steps between 2 failures).
* aclink: Events that occurred at the neighbouring AC links, expressed as a binary variable (0: maintenance activity did not occur and 1: maintenance activity occurred)
* MWh/h: Power exchanges through the line in MWh/h
* rad_hour: solar radiations in W/m2
* hum_hour: humidity in %
* MaxWindSpeed: maximum wind speed in m/s
* Sikt: visibility in meters.

## Description of data and sources

* Maintenance, Failure and aclink: European Network of Transmission System Operators for Electricity (ENTSO-E), Transparency Platform - (https://transparency.entsoe.eu/) accessed Aug. 22, 2020
* MWh/h: Energinet, Energi Data Service - (https://www.energidataservice.dk) accessed Aug. 22, 2020.
* rad_hour, hum_hour, MaxWindSpeed, and Sikt: Swedish Meteorological and Hydrological Institute (SMHI), Meteorologiska observationer - (https://www.smhi.se) accessed Aug. 22, 2020.

## Pre-processing activities

Missing data have been interpolated, using simple mean when individual data are missing in a variable that changes gradually. If a whole interval of data is missing or the variable is stochastic, time series modeling or linear regression with a correlated variable are used.

## Authors

* **Sylvie Koziel**

## License

This project is licensed under the Creative Commons Zero v1.0 Universal license.
