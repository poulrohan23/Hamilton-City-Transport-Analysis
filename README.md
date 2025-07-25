# Hamilton-City-Transport-Analysis
## Hamilton Walkability and Bikeability Analysis

## Overview
This project analyzes walkability, bikeability, and related infrastructure metrics for the City of Hamilton, Ontario, as part of the "WorkWalk & BikeBoost" program. The goal is to identify areas with high potential for promoting walking and cycling, assess employment land density, evaluate the young worker population (aged 16-45), calculate mode shift potential, and propose intervention sites to encourage sustainable transportation. The analysis integrates various geospatial datasets and generates an interactive web-based map for visualization and decision-making.

The project uses Python for data processing and visualization, leveraging libraries such as `geopandas`, `pandas`, `shapely`, and `folium`. The output is an HTML file (`hamilton_walkability_bikeability.html`) that provides an interactive map with layers for walkability scores, bikeability scores, employment density, young worker distribution, mode shift potential, and proposed intervention sites.

## Project Goals
- **Walkability and Bikeability Assessment**: Calculate scores based on sidewalk length, street lights, bus stops, bike lanes, and other amenities to identify walkable and bikeable areas.
- **Employment Lands Density**: Analyze the distribution of employment lands across wards to prioritize areas with high employment potential.
- **Young Worker Population**: Estimate the percentage of the population aged 16-45 to target areas with a high proportion of potential active commuters.
- **Mode Shift Potential**: Evaluate the potential to shift car trips to walking or cycling based on demographic and infrastructure data.
- **Intervention Sites**: Propose locations for interventions (e.g., WorkWalk Challenge Start Points, BikeBoost Reward Hubs) in target wards (1, 2, 3, 5).
- **Improvement Suggestions**: Provide recommendations for transit, walkability, and bikeability enhancements in low-scoring areas.

## Data Sources
The analysis uses the following geospatial datasets (expected as GeoJSON files):
- `Street_Light_Poles_and_Luminaires`
- `Traffic_Collisions`
- `hamilton_bike_lanes_osm`
- `hamilton_pedestrian_osm`
- `hamilton_streets_osm`
- `Road_Sidewalk`
- `Street_Centreline`
- `Transit_Service_Areas`
- `HSR_Bus_Stops`
- `Hospitals`
- `EMS_Stations`
- `Police_Stations`
- `Educational_Institutions`
- `Municipal_Services_Centres`
- `Places_of_Worship`
- `Arenas`
- `Spray_Pads`
- `Libraries`
- `Museums_and_Galleries`
- `Public_Art_and_Monuments`
- `City_Waterfalls`
- `Recreation_and_Community_Centres`
- `Park_Sports_Fields`
- `Campgrounds`
- `Ward_Boundaries`
- `Bikeways`
- `Bike_Parking`
- `Hamilton_Bike_Share_Incorporated_Hubs`
- `Hamilton_Bike_Share_Incorporated_Service_Areas`
- `City_Growth_Targets_Population`
- `Addresses`
- `Employment_Lands`
- `Census_Population_Age_and_Gender`

Additionally, Travel Time Survey (TTS) data is hardcoded for wards 1, 2, 3, and 5 to support mode shift calculations.

## Setup Instructions

### Prerequisites
- Python 3.11 or later
- Required Python libraries:
  - `geopandas`
  - `pandas`
  - `shapely`
  - `tqdm`
  - `folium`
- A web browser to view the generated HTML file

### Installation
1. Clone or download this repository to your local machine.
2. Navigate to the project directory in a terminal.
3. Install the required Python libraries using pip:
   ```bash
   pip install geopandas pandas shapely tqdm folium
