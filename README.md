
# 🌲 GIS Suitability Analysis: Pine Tree Viability in North Texas

## Overview

This project explores the ecological suitability of growing Christmas tree species — specifically **Virginia Pine** (*Pinus virginiana*) and **Eastern White Pine** (*Pinus strobus*) — within a 150-mile radius of Dallas, TX.

## Objective

To determine if specific areas in North Texas can support the growth of either tree species using key environmental criteria.

## Data & Methods

- **Data Sources**: USDA Forest Service ecology reports; GIS layers for:
  - Average Annual Temperature (°C)
  - Average Annual Precipitation (mm)
  - Soil pH
  - Elevation (m)

- **GIS Tools**:
  - ArcGIS Pro
  - Raster Calculator
  - Ordinal scoring system (0 = not suitable, 1 = somewhat suitable, 2 = suitable)
  - Combined suitability score: 0–8

- **Visualization**: Two raster maps were created with green-to-red shading to represent suitability for each tree species.

## Results

- **Best suited areas**: East Texas, especially around Tyler, showed the highest suitability scores.
- **Key limiting factor**: Temperature was the most restrictive, with nearly all temperature zones scoring 0 due to North Texas's warmer climate.
- **Virginia Pine** had a broader viability range than Eastern White Pine.

## Reflection

A follow-up analysis might assign greater weight to temperature due to its high limiting effect. Future changes in climate may further impact viability.

## Report

📄 Full write-up: *Pine_Trees_Capability_Analysis_2025_02_19.docx*
