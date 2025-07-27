# 🏙️ Welcome! 
I'm Will Georgia, a Master’s student in Urban Analytics at Georgia Tech with a passion for cities, transportation, and all components of the built environments we share. This portfolio showcases skills I’ve developed through hands-on coursework and case studies.

---

# 🚍 Park-and-Ride Travel Time Simulation

This assignment analyzed park-and-ride travel times from census tract centroids in the Atlanta area to Midtown Station using:

- GTFS transit data from MARTA
- ACS demographic data
- OpenStreetMap road networks
- Spatial network analysis with `sfnetworks`
- Transit routing with `tidytransit`

**Explore the full report here:**

👉 [View Interactive Report on RPubs](https://rpubs.com/wgeorgia6/1238230)

## 📌 Key Tools and Methods

- `tidytransit` and `gtfsrouter` for GTFS data
- `osmdata` and `sfnetworks` for street networks
- `tidycensus` for ACS data (household income & race)
- Spatial joins, centroid extraction, and travel time simulation

## 🗺️ Outputs

The report includes thematic maps and scatterplots showing relationships between:
- Household income and travel time
- Minority population share and travel time

---

# 📊 Analyzing MARTA GTFS Data in R

This project demonstrates how to work with General Transit Feed Specification (GTFS) data from the Metropolitan Atlanta Rapid Transit Authority (MARTA) using R.

🛰️ **Key Tools Used:**
- `tidytransit` for GTFS data handling  
- `sf` and `tmap` for spatial visualization  
- `leaflet` for interactive mapping  
- `dbscan` and `sfnetworks` for spatial clustering and network analysis

🔗 **View the full interactive report on RPubs:**  
👉 [RPubs: MARTA GTFS Analysis](https://rpubs.com/wgeorgia6/1245484)

---

## 🧠 Project Highlights

- Downloaded and parsed MARTA’s live GTFS feed.
- Filtered stop times for specific date/time ranges.
- Mapped stops, routes, and spatial patterns using `leaflet` and `tmap`.
- Used `sfnetworks` and `dbscan` for identifying clusters and patterns in transit stop locations.

---

# 🚇 Change in Public Transit Ridership Near MARTA Rail Stations (2018–2023)

![Change in Ridership Map](Chg_Ridership_near_MARTA_Rail.jpg)

## Overview

This map visualizes the **change in public transit commuting near MARTA rail stations in Atlanta** between 2018 and 2023. Using data from the **American Community Survey (ACS) 5-Year Estimates**, it focuses on areas **within a 1-mile buffer** around each rail station, representing a typical walkable catchment area.

The analysis compares the **percentage of workers commuting by public transit** in 2018 vs. 2023 to identify stations with the most significant changes over time.

## Key Takeaways

- Northern Red Line stations experienced **steep declines**, with some stations seeing reductions over 75%.
- Several central stations show **moderate decreases**, while one even saw **gains in transit mode share**.
- These patterns reflect broader shifts in commuting behavior, likely influenced by **COVID-19**, the **rise of remote work**, and ongoing changes in transit accessibility.

## Methodology

All geospatial analysis was conducted using **ArcGIS Pro**, supported by ACS data accessed via R’s `tidycensus` package.

### 🔧 ArcGIS Geoprocessing Tools Used:

- **Buffer** – Created 1-mile buffers around each MARTA station.
- **Select Layer By Attributes** – Filtered census block groups relevant to the years 2018 and 2023.
- **Intersect** – Identified block groups that intersect each station's buffer.
- **Join Field** – Merged ACS data fields for 2018 and 2023.
- **Calculate Field** – Computed percent change in public transit commuting.
- **Select by Attributes** – Isolated top 5 increases and top 5 decreases in mode share.
- **Labeling with Callouts** – Labeled percent change using Maplex engine and custom halos for legibility.
- **Symbology** – Colored buffers to indicate increase (green) or decrease (orange) in transit usage.

## Design Choices

- **Station names are intentionally omitted** to maintain a clean layout and emphasize the magnitude and geography of change.
- Color-coded **callout labels** highlight the top 5 stations with the **largest increases** and **largest decreases** in transit commuting share.
- A custom legend clarifies MARTA rail lines, buffer zones, and top-performing stations.

## Data Sources

- **ACS 5-Year Estimates (2014–2018 and 2019–2023)**: Table B08301 (Means of Transportation to Work), accessed via [`tidycensus`](https://walker-data.com/tidycensus/) in R.
- **MARTA Station and Rail Line GIS Data**: Georgia GIS Clearinghouse and MARTA Open Data Portal.

## Tools Used

- ArcGIS Pro 3.x
- R (for ACS data extraction and prep)

---

## 🌲 GIS Capability Analysis: Pine Tree Viability in North Texas

**Objective:** Can Christmas trees grow near Dallas, Texas? Let's use GIS tools to conduct a capability analysis to find out.

**Approach:**
- Compared native habitat conditions of **Virginia Pine** and **Eastern White Pine** to North Texas environmental data.
- Pulled geospatial layers on temperature, precipitation, soil pH, and elevation.
- Classified each factor into ordinal ranks (0 = not suitable to 2 = suitable).
- Combined layers using Raster Calculator in ArcGIS Pro to score overall viability (0–8 scale).

**Outcome:**  
Viable areas were concentrated in East Texas, with temperature being the most limiting factor across the study area.

📄 [Read the Full Report](./Pine_Trees_Capability_Analysis_2025_02_19.pdf)

---

## 🗺️ GIS StoryMap: Dallas Parks: Decent or Deficient?

**Overview:**  
This ArcGIS StoryMap gives looks at one component factoring into Dallas' poor ranking in public green space.

**Features:**
- Map-based storytelling using **ArcGIS StoryMaps**
- Feature layers pulled from the city of Dallas and the Census Bureau
- Geoprocessing tools used to take a closer look at park coverage in the city by census tract

🔗 [Explore the StoryMap](https://arcg.is/1aO1Cv1)

---

## 📬 Contact

- 📧 william.georgia@gatech.edu
- 🌐 [wpgeorgia.github.io/portfolio/]
