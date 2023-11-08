# Power outages in 2019, California and the impact on medically vulnerable populations
Data and scripts for California 2019 power outage and medically vulnerable population analysis

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
- Identifying power outage events at different lengths
  - 1-8 hours, 9-24 hours, 24+ hours
  - Code
- Calculating the number of customers who experienced power outage events at different lengths
  - Code 
- Creating a bi-variate map showing
  1. the % of customers who experienced at least one 24+ hours power outage event
  2. % of DME users out of total population
  - Code
- Creating a bi-variate map showing
  1. the % of customers who experienced at least one 24+ hours power outage event
  2. the % of people under 200% Federal Poverty Line (FPL)

## Result data
- Data for Exhibit 1
- Data for Exhibit 2
