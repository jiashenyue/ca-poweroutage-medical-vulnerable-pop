# Power outages in 2019, California and the impact on medically vulnerable populations


A work of [CrisisReady](https://www.crisisready.io/) team

Data and scripts for California 2019 power outage and medically vulnerable population analysis.

## Data for analysis
- Data of customers out of power
  - Purchased from [poweroutage.us](https://poweroutage.us/)
- Medical vulnerability
  - Medically vulnerable population in this study is defined in this study as the users of durable medical equipment (DME) among Medicare beneficiaries
  - Data of this metric is available from [emPOWER](https://empowerprogram.hhs.gov/) platform of Department of Human and Health Services [(HHS)](https://www.hhs.gov/)
- Healthcare resource availability
  - The following metrics are retrieved from Health Center Program Uniform Data System [(UDS)](https://data.hrsa.gov/tools/data-reporting/program-data) by the Health Resources and Services Administration [(HRSA)](https://www.hrsa.gov/)
    - Penetration rate of healthcare providers as a member of the Health Center Program [(HCP)](https://bphc.hrsa.gov/) of HRSA at the ZIP code level
    - Percent of population served by each HCP member
    - Percent of population under federal poverty line
- Geographical boundaries
  - County boundaries for analysis and result reporting
    - [U.S. Census TIGER](https://www.census.gov/geographies/mapping-files/time-series/geo/tiger-line-file.html)
  - Census-designated places (CDP) for data laundry of customers experiencing power outages
    - [U.S. Census TIGER](https://www.census.gov/geographies/mapping-files/time-series/geo/tiger-line-file.html)

## Analysis conducted
- Convert the original poweroutage.us data to long form
  - [Code](https://github.com/jiashenyue/ca-poweroutage-medical-vulnerable-pop/blob/main/code/00_long_form_data_gen.nb.html)
- Identifying power outage events at different lengths and calculate the numbers of customers affected
  - [Code](https://github.com/jiashenyue/ca-poweroutage-medical-vulnerable-pop/blob/main/code/01_generate_outage_events.nb.html)
- Creating a bi-variate map showing
  1. the % of customers who experienced at least one extreme power outage event
  2. % of DME users out of total population
  - [Code](https://github.com/jiashenyue/ca-poweroutage-medical-vulnerable-pop/blob/main/code/04_bivariate_county_map.nb.html)
- Creating a scatterplot showing
  1. the % of customers who experienced at least one extreme hour power outage event
  2. % of DME users out of total population
  - [Code](https://github.com/jiashenyue/ca-poweroutage-medical-vulnerable-pop/blob/main/code/05_scatterplot_extreme_events_medically_vulnerables.nb.html)
- Creating a scatterplot showing
  1. the % of customers who experienced at least one extreme power outage event
  2. the % of people under 200% Federal Poverty Line (FPL)
  - [Code](https://github.com/jiashenyue/ca-poweroutage-medical-vulnerable-pop/blob/main/code/06_scatterplot_extreme_events_low_income.nb.html)

## Result data
- Long-form time series of customers experiencing a power outage in counties of California, 2019
  - Download data from [Zenodo](https://zenodo.org/records/10198709)
- All power outage events in California, 2019
  - [CSV file](https://github.com/jiashenyue/ca-poweroutage-medical-vulnerable-pop/blob/main/result/power-outage-events/ca_pct_household_oop_new_def.csv)
- Esri Shapefiles of power outage events by county
  - [Folder](https://github.com/jiashenyue/ca-poweroutage-medical-vulnerable-pop/tree/main/result/shapefile-power-outage-diff-length)

## Sample exhibits

![image](https://github.com/jiashenyue/ca-poweroutage-medical-vulnerable-pop/blob/main/plot/01_bivariate_map.png)
