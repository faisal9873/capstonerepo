## Energy Consumption Prediction in the Home ##

### Introduction ###

**Introduction** 
This year, at the height of winter and due to extreme cold, the Alberta grid was overstretched, prompting the 
[Alberta Electric System Operator (AESO)](https://globalnews.ca/news/10231766/alberta-grid-concerns-critical-infrastructure/)  
to issue calls for people to limit energy use. This urgent appeal came as several power facilities were on the brink of 
collapse, posing a significant risk of rolling blackouts. Additionally, B.C. Hydro experienced surging electricity demand, setting new records.
Despite the critical infrastructure being managed by the three tiers of government and select public and private sector 
groups, every individual plays a crucial role as a stakeholder in this industry and should be empowered to contribute to 
its resilience and sustainability. This responsibility begins within every household, where a comprehensive understanding 
of energy consumption habits can collectively exert a significant influence on bolstering the grid's overall resilience 
and stability. This was the motivation behind leveraging machine learning to understand energy consumption patterns.

**Problem Statement**
We lack a comprehensive understanding of how energy is utilized by the appliances in our homes.

**Our Solution**
Develop predictive models to help us understand the relationship between appliances energy consumption and predictors.

**Objective**
The aim of this project is to utilize energy data obtained from household appliances to 
predict expected energy consumption. This endeavor offers several benefits. 

**Potential Impact** 
Firstly, homeowners can accurately size photovoltaics and battery energy storage systems based on the predictions to 
accommodate additional load. Secondly, detecting and addressing unhealthy usage patterns can lead to a reduction in 
energy expenditure.

**Dataset**
We will be using a real world energy dataset of a [house](https://www.sciencedirect.com/science/article/pii/S0378778816308970?via%3Dihub) 
containing energy consumed, logged in ten minutes interval for a toal of 137 days. The dataset contains information 
about energy consumption of appliances used in the home such as heat recovery ventilation unit, domestic hot water pump, 
the energy consumption of appliances, lighting, and electric baseboard heaters. The dataset also contains the weather 
condition at the time of recording, estimated by using the weather measurments from the nearest airport weather station 
(Chièvres Airport, Belgium), located within 12 km of the house. 


**Data Dictionary**
To help us with our analysis, we take some time to study the data dictionary below. 

Energy data of appliances:
- Appliances energy consumption (numeric) (Wh)
- Light energy consumption (numeric) (Wh)

Weather data
- T1, Temperature in kitchen area (numeric) (&deg;C)
- RH1, Humidity in kitchen area (numeric) (%)
- T2, Temperature in living room area (numeric) (&deg;C)
- RH2, Humidity in living room area (numeric) (%)
- T3, Temperature in laundry room area (numeric) (&deg;C)
- RH3, Humidity in laundry room area (numeric) (%)
- T4, Temperature in office room (numeric) (&deg;C)
- RH4, Humidity in office room (numeric) (%)
- T5, Temperature in bathroom (numeric) (&deg;C)
- RH5, Humidity in bathroom (numeric) (%)
- T6, Temperature outside the building (north side) (numeric) (&deg;C)
- RH6, Humidity outside the building (north side) (numeric) (%)
- T7, Temperature in ironing room (numeric) (&deg;C)
- RH7, Humidity in ironing room (numeric) (%)
- T8, Temperature in teenager room 2 (numeric) (&deg;C)
- RH8, Humidity in teenager room 2 (numeric) (%)
- T9, Temperature in parents room (numeric) (&deg;C)
- RH9, Humidity in parents room (numeric) (%)
- To, Temperature outside (from Chièvres weather station) (&deg;C)
- Pressure (from Chièvres weather station) (numeric) (mmHg)
- RHo, Humidity outside (from Chièvres weather station) (numeric)(%)
- Windspeed (from Chièvres weather station) (numeric) (m/s)
- Visibility (from Chièvres weather station)
- Tdewpoint (from Chièvres weather station) (numeric) (&deg;C)

Other data
- Random Variable 1 (RV_1) (numeric) (dimensionless)
- Random Variable 2 (RV_2) (numeric) (dimesnsionless)
- Number of seconds from midnight (NSM) (numeric) (s)
- Week status (weekend (0) or a weekday (1)) (categorical)

Date data
- Day of week (Monday, Tuesday… Sunday) (categorical)
- Date time stamp

Field of interest:
- Appliances energy consumption (numeric) (Wh)

