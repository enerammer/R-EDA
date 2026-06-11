---
title: "Data set"
---

In order to demonstrate how to work with Excel Workbooks, we provide the data as such:

[Download](https://raw.githubusercontent.com/KUBDatalab/R-EDA/main/episodes/data/flightdata.xlsx)

Data is sourced from the `nycflights13` package, and collated into the workbook. It is supplemented with 
relevant IATA codes from [datahub.io](https://datahub.io/core/airport-codes).

The `nycflights13` data is originally extracted from 
[Bureau of Transportation Statistics](https://www.transtats.bts.gov/DL_SelectFields.asp?Table_ID=236).


FAA Aircraft registry, https://www.faa.gov/licenses_certificates/aircraft_certification/aircraft_registry/releasable_aircraft_download/

The workbook consist of four spreadsheets:

## Flights

|  Variable  |  Description/Code                               | Unit   |   
|------------|-------------------------------------------------|--------|
|  year    |  Year of departure  |        |
|  month        | Month of departure                                       |        |
|  day  | Day (of month) of departure                              |  |
|  dep_time  | Actual departure time, format HHMM or HMM in local timezone                              |  |
|  sched_dep_time    | Scheduled departure time, format HHMM or HMM in local timezone| |
|  dep_delay    | Departure delay. Negative values represent early departure| minutes   |
|  arr_time   | Actual arrival time, format HHMM or HMM in local timezone  |  |
|  sched_arr_time   |  Scheduled arrival time, format HHMM or HMM in local timezone |  |
|  arr_delay   |  Arrival delay. Negative values represent early departure | minutes |
|  carrier   | Two letter carrier abbreviation. Matches the carrier variable in "airlines"  |  |
|  flight   | Flight number   |  |
|  tailnum   | Plane tail number. Matches the tailnum variable in "planes"  |  |
|  origin   | iata code for origin airport. Mathces the iata_code variable in "airports"  |  |
|  dest   | iata code for destination airport. Mathces the iata_code variable in "airports"   |  |
|  air_time   | Amount of time spent in the air  | minutes  |
|  distance   | distance between airports  | miles  |
|  hour   | Time of scheduled departure - the hour part  |  |
|  minute   | Time of scheduled departure - the minutes part  |  |
|  time_hour   | Schedules date and hour of the flight as POSIXct date. Can join flights data to "weather" data along with the origin variable  |  |

## airlines

|  Variable  |  Description/Code                               | 
|------------|-------------------------------------------------|
|  carrier    |  Two letter abbreviation of the carrier. Matches the carrier variable in "flights"  |       
|  name        | Full name of the carrier                                        |        

## planes

|  Variable  |  Description/Code                               | Unit   |   
|------------|-------------------------------------------------|--------|
|  tailnum    | Tail number. Matches the tailnum variable in "flights"   |        |
|  year        | Year the plane was manufactured                                       |        |
|  type  |  Type of plane. Either fixed wing with multiple or single engine, or rotorcract (helicopter)                            | |
|  manufacturer  |  Manufacturer of the plane                             | |
|  model  | Model of the plane                              | |
|  engines  |  Number of engines                              | |
|  seats  | Number of passenger seats                               | |
|  speed  | Average cruising speed                              | miles/h|
|  engine  |  type of engine                             | |

## Weather

|  Variable  |  Description/Code                               | Unit   |   
|------------|-------------------------------------------------|--------|
|  origin    |    |        |
|  year    |    |        |
|  month    |    |        |
| day    |    |        |
|  hour    |    |        |
| temp    |    |        |
|  dewp    |    |        |
|  humid    |    |        |
|  wind_dir    |    |        |
|  wind_speed    |    |        |
|  wind_gust    |    |        |
|  precip    |    |        |
|  pressure    |    |        |
|  visib    |    |        |
|  time_hour    |    |        |


## iata_codes

Skal konsolideres med "airports" data fra nycflights13

|  Variable  |  Description/Code                               | Unit   |   
|------------|-------------------------------------------------|--------|
|  iata_code    |    |        |
|  ident    |    |        |
|  type    |    |        |
|  name    |    |        |
|  elevation_ft    |    |        |
|  continent    |    |        |
|  iso_country    |    |        |
|  iso_region    |    |        |
|  municipality    |    |        |
|  icao_code    |    |        |
|  gps_code    |    |        |
|  local_code    |    |        |
|  lat    |    |        |
|  long    |    |        |