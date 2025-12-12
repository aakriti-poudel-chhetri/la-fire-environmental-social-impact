# Visualizing fire scars through false color
## A case of Eaton and Palisades fires

## Introduction
In January 2025, the Eaton and Palisades fires ignited almost simultaneously in the foothills and coastal wildland–urban interface zones of Los Angeles County, triggered by anomalously dry conditions and strong Santa Ana winds in Los Angeles County, California. These concurrent events burned more than 38 000 acres and destroyed over 16 000 structures resulting in around 30 direct fatalities and mass evacuations affecting more than 150, 000 individuals.

![Eaton Palisades Fires](https://freeseandgoss.com/wp-content/uploads/2025/01/palisades-and-eaton-fires--scaled.jpeg)
*Figure 1: Extent of damage from Eaton and Palisades fires in Los Angeles County. / Source: [Freese and Goss](https://freeseandgoss.com/pacific-palisades-eaton-fires/)*

## Environmental Impact
The Eaton and Palisades fires had profound environmental consequences across terrestrial, atmospheric and aquatic systems. Air quality deteriorated sharply, with PM2.5 concentrations exceeding 400 µg/m³, contributing to a prolonged hazardous air quality episode that extended far beyond the immediate burn zones. The combustion of built structures released complex mixtures of pollutants, including fine particulates and heavy metals such as lead, raising concerns about toxic exposures both outdoors and within impacted neighborhoods. Post‑fire runoff mobilized ash, sediment and chemical pollutants into waterways, contributing to soil and water contamination altering nutrient cycling and disrupting aquatic ecosystems. These severe environmental impacts shows  how urban wildfires are  interconnected, especially when fires consume both natural vegetation and human-made materials.

## Social Impact
The social impacts of the January 2025 wildfires were extensive and unevenly distributed. Beyond widespread property damage and environmental degradation, these events disproportionately affected socially vulnerable populations, including low-income households, older adults, renters, and individuals with limited access to healthcare and transportation. Delays in evacuation, long exposure to smoke, losing homes, and disruptions to basic services made existing social and health problems worse. Community groups and public services struggled to meet the rising demand for emergency help, housing and mental health support. These fires show that urban wildfire risk is not just an environmental problem but it is also a common social issue, affected by inequalities that shape who is exposed, how well people can cope, and how they recover.

## Objective

The objective of this assignment is to
- produce a false-color image of the Eaton and Palisades fires using remote sensing data.
- highlight the burn scar.
- demonstrate how coding and data visualization support environmental monitoring.
- perform environmental justice analysis by using spatial joins and clipping to examine socioeconomic vulnerability in the burn-affected areas.

## Repository Structure
```
la-fire-environmental-social-impact/
│
├── README.md
├── eaton-palisades-fire.ipynb
└── .gitignore
     └───data
         ├── Eaton_Perimeter_20250121
         ├── Palisades_Perimeter_20250121
         └── landsat8-2025-02-23-palisades-eaton.nc

```

## Data

A `data/` directory is created inside the `la-fire-environmental-social-impact` repository. Due to the large size of data, the data folder is included in `.gitignore` and is not tracked by version control.

In this assignment, we will be using the following datasets.

### Simplified collection of bands from the Landsat Collection 2 Level-2
The first dataset is a simplified collection of bands (red, green, blue, near-infrared and shortwave infrared) from the Landsat Collection 2 Level-2 atmosperically corrected surface reflectance data, collected by the Landsat 8 satellite.

The data was retrieved from the [Microsof Planetary Computer data catalogue](https://planetarycomputer.microsoft.com/dataset/landsat-c2-l2) and clipped to an area surrounding the fire perimeters.

### Fire perimeters for the Eaton and Palisades fires
The second dataset is of fire perimeters for the Eaton and Palisades fires, and is retrieved from the [County of Los Angeles Open Data](https://data.lacounty.gov/). The data can be accessed from the [link](https://data.lacounty.gov/maps/ad51845ea5fb4eb483bc2a7c38b2370c/about).

### Environmental Justice Index (EJI) data
The EJI data is extracted from [Centers for Disease Control and Prevention and Agency for Toxic Substances Disease Registry](https://atsdr.cdc.gov/place-health/php/eji/eji-data-download.html)). It provides information on census tract-level demographic and socioeconomic data. This study uses the 2024 California EJI dataset to look at the racial makeup of communities affected by fires, based on the proportion of minority populations.

## Data Citation
*Landsat Collection 2 Level-2*. Microsoft Planetary Computer. Retrieved 15 Nov, 2025. https://planetarycomputer.microsoft.com/dataset/landsat-c2-l2.

*Palisades and Eaton Dissolved Fire Perimeters*. (2025) County of Los Angeles Open Data. https://data.lacounty.gov/maps/ad51845ea5fb4eb483bc2a7c38b2370c/about.

*Why Is That Forest Red and That Cloud Blue?*. (2014, March 4). NASA Earth Observatory. https://earthobservatory.nasa.gov/features/FalseColor.

*What Are the Band Designations for the Landsat Satellites?*.(2025, July 11). U.S. Geological Survey. https://www.usgs.gov/faqs/what-are-band-designations-landsat-satellites.

*Common Landsat Band Combinations*. (2021, November 12). U.S. Geological Survey. https://www.usgs.gov/media/images/common-landsat-band-combinations

*Centers for Disease Control and Prevention and Agency for Toxic Substances Disease Registry*. Environmental Justice Index. Accessed 2025, November 21. https://atsdr.cdc.gov/place-health/php/eji/eji-data-download.html

## References

This repository contains materials for the blog post of [final project](https://meds-eds-220.github.io/MEDS-eds-220-course/assignments/final-project.html) for the course [EDS 220 - Working with Environmental Datasets](https://meds-eds-220.github.io/MEDS-eds-220-course/). This course is part of the [UCSB Masters in Environmental Data Science](https://bren.ucsb.edu/masters-programs/master-environmental-data-science).

### Course Information
 - **Course Title:** EDS 220 - Working with Environmental Datasets
 - **Term:** Fall 2025

#### Teaching Team:
- **Instructor:** Dr. Carmen Galaz García

- **Co-instructor**: Dr. Annie Adams

**Author:** Aakriti Poudel