# Zambia Energy Access Analysis

Zambia is a landlocked country in central Africa with a population of 21.31 million people. The country's energy mix is heavily dependent on Hydropower which has seen a lot of pressure due to effects of climate change such as the recent drought which was the worst recorded drought in the country's history. Being a developing country, Zambia is still making strides in providing adequate electricity for its citizens, a big aspect of this is reaching all corners of the country through the establishment of power infrastructure. The country, through an act of Parliament of 2003, established the Rural Electrification Authority (REA) with the sole goal to drive electricty access to underserved corners of the country. Unfortunately, this is still far from being the case, according to the REA [official website](https://www.rea.org.zm/remp/), the rural electrification access rate stands at only 8.1% overall. 

In it's Rural Electrification Master Plan (REMP), REA has focused its efforts on electrifying 1,217 Rrual Growth Centers, which are designated areas with concentrated populations and economic activity. Through this approach, REA had achieved an electrification rate of these centers of 45% as of 31st Mach, 2024! 

In this notebook we seek to explore this use case with open data and workflows powered by Github Copilot!

## Overview

The `energy_access.ipynb` notebook creates a multi-layered geospatial visualization that helps identify areas with potential energy access gaps in Zambia by overlaying:

1. **Population Density** - Shows where people live using WorldPop data
2. **Power Lines Network** - Maps the electrical transmission grid by voltage level
3. **Substations** - Plots locations of electrical substations
4. **10km Service Areas** - Visualizes potential energy access coverage with 10km radius buffers around substations

## Key Features

- Downloads and processes population density data from WorldPop
- Fetches power infrastructure data from OpenStreetMap using Overpass API
- Creates individual and combined visualizations with proper layering
- Implements GIS analysis techniques to estimate energy access coverage
- Visualizes different voltage levels in the transmission network

## Technologies Used

- **Python Libraries**: GeoPandas, Matplotlib, Rasterio, NumPy, Overpy
- **Data Sources**: WorldPop, OpenStreetMap
- **Spatial Analysis**: Coordinate system transformations, buffering, geometric operations

## How to Use

1. Clone this repository
2. Ensure required dependencies are installed
3. Run the Jupyter notebook to generate visualizations
4. The notebook will automatically download required population density data

## Output

The final visualization creates an integrated map showing population density with power infrastructure overlaid. Yellow 10km buffers around substations help identify which populated areas have potential access to electricity and which areas may not.
