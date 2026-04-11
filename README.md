# New-England-Airports-Analysis

**Bentley University Computer Information Systems | CS230 Data Analysis Project**

## Overview
Interactive Streamlit dashboard analyzing airports across New England (CT, MA, ME, NH, RI, VT). Filter by **airport type** (small, medium, large) and **location** (state/region) to explore data visualizations.

## Sample Data Needed
Download New England airport data from [OurAirports.com](https://ourairports.com/data/) or use any CSV with columns:
- type, iso_region, latitude_deg, longitude_deg, elevation_ft

**Live Demo**: [vs-airport-analysis.streamlit.app](vs-airport-analysis.streamlit.app)

## Features
- 📊 **Interactive Data Table** - Sort airports by any column (elevation, coordinates, type)
- 🗺️ **Interactive Map** - PyDeck visualization of airport locations using lat/long
- 📈 **Dual Bar Charts**:
  - Matplotlib: Basic airport type counts
  - Plotly: Advanced hover details + dark theme
- 🏔️ **Top 5 Highest Airports** - Ranked by elevation_ft
- 🔍 **Sidebar Filters** - Type + location selection

## Tech Stack

## Data Source
`us-airports.csv` - Contains airport metadata including:
- `type` (small_airport, medium_airport, large_airport, etc.)
- `iso_region` (state codes: US-CT, US-MA, etc.)
- `latitude_deg`, `longitude_deg`, `elevation_ft`

## Key Challenges Solved
- CSV parsing + numeric type conversion (lat/long, elevation)
- Error handling for missing columns/data
- Interactive filtering with real-time chart updates
- Dual visualization approaches (static vs interactive)

## Setup & Run Locally
```bash
pip install streamlit pandas plotly matplotlib pydeck
streamlit run Final.py
```

---
**Built by Victoria Saintil** - Aspiring Application Developer
