# 🏙️ Welcome! 
I'm Will Georgia, a Master’s student in Urban Analytics at Georgia Tech with a passion for cities, transportation, and all components of the built environments we share. This portfolio showcases skills I’ve developed through hands-on coursework and case studies.

---

## 🌲 GIS Suitability: Pine Tree Viability in North Texas

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

## 🗺️ StoryMap: Dallas Parks: Decent or Deficient?

**Overview:**  
This ArcGIS StoryMap gives looks at one component factoring into Dallas' poor ranking in public green space.

**Features:**
- Map-based storytelling using **ArcGIS StoryMaps**
- Feature layers pulled from the city of Dallas and the Census Bureau
- Geoprocessing tools used to take a closer look at park coverage in the city by census tract

🔗 [Explore the StoryMap](https://arcg.is/1aO1Cv1)

---

# 🚍 Park-and-Ride Travel Time Simulation

This assignment analyzes park-and-ride travel times from census tract centroids in the Atlanta area to Midtown Station using:

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

## 📬 Contact

- 📧 william.georgia@gatech.edu
- 🌐 [wpgeorgia.github.io/portfolio/]
