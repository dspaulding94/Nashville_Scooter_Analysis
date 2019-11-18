
## **Nasvhille Scooter Analysis**

**Summary:**\
Nashville's department of urban planning is interested to find an ideal density and count of scooters to its residents, without over-crowing sidewalks and streets.

This project was a class assignment where teams of four decided which aspects of the project to pursue. My team reviewed the quality of data provided by the micro-mobility providers.

**Team Goal**\
Identify which scooter providers provide the most accurate information per city's ordinances. 

**Per Ordinance:**\
All permitted operators will first clean data before providing or reporting data to Metro. Data 
processing and cleaning shall include:  
 1. Removal of staff servicing and test trips
 2. Removal of trips below one minute
 3. Trip lengths are capped at 24 hours
Anecdotally, per metro ITS staff, some of these observations may still be in the data.

**The Data**\
Shared Urban Mobility Device (SUMD) availability data for May, June, and July 2019:
1. .May data shape:  (20292503, 9)
2. June data shape:  (28046095, 9)
3. July data shape:  (25075445, 9)

pubdatetime - date and time that the device was polled\
latitude - latitude location of device when polled\
longitude - longitude location of device when polled\
sumdid - unique identifier for the device\
sumdtype - one of two types (powered or standard)\
chargelevel - battery charge level of the device when polled\
sumdgroup - type of device (scooter or bicycle)\
costpermin - the cost per minute of device use\
companyname - the company that owns the device\

**Findings:**\
A sizable number of trips reported by operators do not meet ordinance requirements.
* Over 6,900 trips lasted longer than 24 hours.
* Over 9,000 trips lasted less than a minute.
* Over 79,000 trips have a distance under 3 meters.
* One provider reported the majority of non-compliant data.
* One name is shared by multiple scooters.

