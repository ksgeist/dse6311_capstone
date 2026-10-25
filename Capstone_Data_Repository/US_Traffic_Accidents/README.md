# README

## Dataset description
This project investigates how roadway, temporal, environmental, and weather conditions are associated with motor-vehicle crash occurrence or severity using publicly available U.S. transportation data. Students will combine crash records from the National Highway Traffic Safety Administration (NHTSA), part of the U.S. Department of Transportation, with historical weather observations from the National Oceanic and Atmospheric Administration (NOAA) and potentially the U.S. Census for population density and commuter-density measures. Primary uses could include:

- identifying weather and roadway conditions associated with more severe crashes
- modeling crash severity using temporal, environmental, and roadway features
- examining how precipitation, visibility, temperature, wind, or winter conditions relate to crash patterns
- developing reproducible geospatial and temporal data-integration workflows for transportation safety analysis
- integrating commuter data from the U.S. Census would be a novel improvement, but is not required

A key scope distinction is that datasets containing only recorded crashes can support analysis of **crash severity or characteristics conditional on a crash being reported**; they cannot, by themselves, estimate the probability that a crash will occur. Estimating crash occurrence requires an appropriate denominator or comparison data representing times and locations without crashes, as well as suitable traffic/exposure information.

Further, if the goal is to predict traffic fatalities from non-fatalities specifically, it will require regional intersection of the FARS and CRSS datasets.

### Possible question
Can weather and road patterns sufficiently predict fatal traffic accident rates from non-fatal ones at the county level?

## Source Citation
National Highway Traffic Safety Administration (NHTSA). Crash Report Sampling System (CRSS). https://www.nhtsa.gov/crash-data-systems/crash-report-sampling-system

National Highway Traffic Safety Administration (NHTSA). Fatality Analysis Reporting System (FARS). https://www.nhtsa.gov/research-data/fatality-analysis-reporting-system-fars

National Oceanic and Atmospheric Administration (NOAA), National Centers for Environmental Information (NCEI). Global Hourly / Integrated Surface Database (ISD). https://www.ncei.noaa.gov/products/land-based-station/integrated-surface-database

## Data documentation
NHTSA provides annual crash data files and coding documentation. CRSS is a sample of police-reported crashes across the United States and its public files do not include precise crash locations. FARS covers fatal crashes and may be more suitable for spatial linkage where usable coordinates and compatible time fields are available. Confirm the selected year's data dictionary and location fields before designing the project.

- CRSS data files and documentation: https://www.nhtsa.gov/file-downloads?p=nhtsa/downloads/CRSS/
- FARS data and documentation: https://www.nhtsa.gov/research-data/fatality-analysis-reporting-system-fars
- NOAA NCEI Global Hourly data: https://www.ncei.noaa.gov/products/land-based-station/integrated-surface-database
- NOAA Climate Data Online API documentation: https://www.ncei.noaa.gov/cdo-web/webservices/v2

## Suggested NOAA weather integration
A practical starting point is NOAA NCEI's Global Hourly station observations, which include variables such as temperature, dew point, wind, visibility, present-weather codes, and precipitation where observed. The CDO API requires a free token; for larger historical extracts, NCEI also provides bulk-download options. Choose weather variables and station coverage based on the crash study period and geography.

Recommended workflow:

1. **Choose the crash source and scope first.** If using CRSS, do not plan an exact crash-to-weather-station join because the public files omit precise crash locations. Consider a state or county-level study using a different source that includes suitable geocoding, or use CRSS for severity modeling without precise NOAA linkage. This will be true if trying to predict fatal vs. non-fatal crash rates.

Alternatively:
1. **Choose a compatible weather source.** For a geocoded crash dataset, identify NOAA stations near each crash location and within the study period. Review station metadata, distance, elevation, and observation completeness.

2. **Match time carefully.** Convert crash timestamps and weather observations to a common time standard, accounting for local time zones and daylight saving time. Match to the nearest preceding observation or a defined window around the crash time, and document the rule.

3. **Create weather features.** Depending on available observations, derive indicators for precipitation, snow, freezing conditions, low visibility, high wind, and temperature. Preserve missingness flags rather than automatically treating missing weather observations as clear conditions.

4. **Assess linkage quality.** Record the distance to the selected station and time difference from the crash. Compare alternative station-selection rules and exclude or flag poor matches.

5. **Avoid causal overclaiming.** Weather and crash severity can be associated with road type, traffic volume, time of day, geography, and driver behavior. A predictive association is not, on its own, a causal effect.

## Suggested project scope
For a feasible capstone, select one state or region and a limited number of years. A geocoded crash source with usable timestamps is needed for a direct NOAA linkage. If using FARS, frame the primary outcome as fatal-crash characteristics or severity among fatal crashes; FARS alone cannot estimate the risk of a crash versus no crash. For a crash-severity study using CRSS, use its sampling design and weights appropriately and do not fabricate precise location-based weather matches.

## Suggested commuter-level surveys from the U.S. Census
The ACS (American Community Survey) polls a subset of Americans in every zipcode every year to estimate the number of commuters (among other things). Population and commuter density, including historical records, could be used to add a novel layer to the analysis that goes beyond incorporating external factors and gets at routine congestion concerns. While it would still not be causal in any way, it could give additional context currently missing from the NHTS datasets.

## Final notes
This is not an entirely novel analysis, but few students tackle multiple dataset joins, which flexes more data muscles, or they do not try to expand the analysis in novel directions. This project is intended to give you new ideas to an old problem to see if you can come up with something insightful. 