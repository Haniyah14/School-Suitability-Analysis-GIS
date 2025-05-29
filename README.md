# School Suitability Analysis for Karachi, Sindh

## Project Overview

This project performs a spatial analysis to identify suitable locations for establishing new schools in the Sindh province of Pakistan, focusing on Karachi and its districts. Using **Google Earth Engine (GEE)**, the analysis integrates multiple spatial datasets including population density, road networks, and existing school locations to evaluate site suitability based on accessibility and population coverage.

---

## Features

- **District Selection:** Interactive dropdown to select any district within Sindh for targeted analysis.
- **Buffer Distance Controls:** Adjustable sliders to set buffer distances around population centers, roads, and existing schools.
- **Suitability Criteria:**
  - Suitable locations must be within specified distances to populated areas and roads.
  - Suitable locations must be sufficiently distant from existing schools to avoid redundancy.
- **Layer Control:** Toggle visibility of roads, schools, and population density layers.
- **Summary Panel:** Displays area statistics for suitable and unsuitable zones.
- **Interactive Map Legend:** Clarifies color codes for suitability, boundaries, and layers.
- **Help Panel:** Provides detailed instructions for users on how to use the tool.

---

## Data Sources

- **Administrative Boundaries:** FAO GAUL 2015 dataset (level 2) for district boundaries.
- **Population Density:** Gridded Population of the World (GPWv4) adjusted population density.
- **Roads:** Custom roads feature collection (user uploaded assets).
- **Existing Schools:** HOTOSM Pakistan education facilities dataset (user uploaded assets).

---

## How to Use

1. **Select District:** Choose a district from the dropdown menu and click **Show** to focus the analysis on that district.
2. **Adjust Buffers:** Use the sliders to specify buffer distances:
    - Population areas (meters): Defines proximity to population clusters.
    - Roads (meters): Defines accessibility from road networks.
    - Schools (meters): Defines minimum distance from existing schools.
3. **Toggle Layers:** Use checkboxes to display or hide population density, roads, and existing schools on the map.
4. **Analyze Results:** Suitable and unsuitable areas are visualized with green and red overlays respectively. Area statistics are shown on the top-right.
5. **Help:** Click the **Help** button for detailed instructions and methodology explanation.

---

## Technologies Used

- **Google Earth Engine (GEE):** Cloud-based geospatial analysis platform for processing and visualizing spatial data.
- **JavaScript:** Used within the GEE code editor environment to create the interactive UI and perform spatial calculations.

---

## Code Highlights

- Interactive UI components built with GEE `ui` module for user-friendly experience.
- Buffer zones created around population clusters, roads, and schools to classify suitable areas.
- Use of `.reduceToVectors()` and `.buffer()` functions for vector spatial operations.
- Dynamic map layers with toggle visibility.
- Area calculations and summary statistics displayed on the UI.
- Custom legend and help panels enhance usability.

---

## Potential Improvements

- Incorporate additional factors such as land use, terrain elevation, and socioeconomic data.
- Extend analysis to other provinces or rural areas.
- Integrate real-time data updates from local authorities.
- Implement automated report generation based on analysis results.

---

## How to Run

1. Open [Google Earth Engine Code Editor](https://code.earthengine.google.com/).
2. Copy the full project script into a new script file.
3. Run the script to load the interactive UI and map.
4. Select districts and adjust parameters as desired.

---

## License

This project is provided for educational and research purposes. Please cite appropriately if used in publications.

---

## Contact

For any questions or collaboration, please reach out at:

- Email: your.email@example.com  
- GitHub: [your-github-username](https://github.com/your-github-username)  

---

*Thank you for exploring this school suitability analysis project using Google Earth Engine!*
