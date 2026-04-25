# Mangrove Water Level Risk Project

## About

This project develops a machine learning-based system to predict flood and water level risk in mangrove ecosystems. By analyzing environmental, hydrological, and geographic factors, the project identifies high-risk areas and events, enabling better disaster preparedness and ecosystem management. The analysis integrates multispectral remote sensing data (NDWI), hydrological measurements, climatic variables, and land-use patterns to assess coastal vulnerability to flooding.

## Project Overview

The **Mangrove Water Level Risk Project** is a data-driven environmental monitoring system that:

- **Predicts water level risks** in mangrove regions using 22 environmental and geographic features
- **Classifies areas** into "High Risk" and "Low Risk" categories
- **Analyzes key drivers** of flooding including rainfall, tide levels, river discharge, and mangrove cover
- **Supports coastal zone management** and climate adaptation planning

## Dataset

The project uses a comprehensive dataset of 100 observations with the following features:

### Geographic & Spatial
- **Latitude, Longitude** - Geographic coordinates of measurement locations
- **Distance_to_Urban_km** - Proximity to urban areas

### Hydrological Variables
- **Water_Level_m** - Current water level in meters
- **Tide_Level_m** - Tidal elevation
- **River_Discharge_cms** - River flow rate in cubic meters/second
- **Groundwater_Level_m** - Subsurface water depth

### Meteorological Data
- **Rainfall_mm** - Precipitation in millimeters
- **Evaporation_mm** - Water evaporation rate
- **Temperature_C** - Air temperature
- **Humidity_%** - Relative humidity percentage
- **Wind_Speed_mps** - Wind speed in meters/second

### Environmental Indicators
- **Soil_Moisture_%** - Soil water content percentage
- **Salinity_ppt** - Water salinity in parts per thousand
- **NDWI** - Normalized Difference Water Index (remote sensing indicator)
- **Mangrove_Cover_%** - Mangrove forest coverage percentage
- **Land_Use_Type** - Categorical land use classification (Urban, Wetland, Forest, Agriculture)

### Event & Temporal Variables
- **Storm_Event** - Boolean flag for storm occurrence
- **Flood_Event** - Boolean flag for flooding occurrence
- **Season** - Seasonal classification (Dry, Wet, Monsoon)

### Target Variable
- **Risk** - Classification label (High Risk / Low Risk)

## Key Features

✅ **Data Processing** - Cleaned and preprocessed environmental data with 100 samples
✅ **Feature Engineering** - 21 environmental and spatial features for prediction
✅ **Risk Classification** - Binary classification of flood risk levels
✅ **Environmental Analysis** - Integration of remote sensing (NDWI) with ground measurements
✅ **Coastal Monitoring** - Comprehensive assessment of mangrove ecosystem health

## Methodology

1. **Data Loading & Exploration** - Loaded CSV dataset with 22 columns
2. **Data Cleaning** - Removed unnecessary temporal fields, handled missing values
3. **Exploratory Analysis** - Statistical analysis of environmental variables
4. **Risk Assessment** - Binary classification of High Risk vs Low Risk scenarios
5. **Model Development** - Machine learning algorithms for risk prediction

## Technical Stack

- **Python 3** - Primary programming language
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computations
- **Matplotlib & Seaborn** - Data visualization

## Usage

The project is implemented as a Jupyter Notebook (`Mangrove_water_level_risk_project.ipynb`) that can be run in Google Colab. Users can:

1. Load mangrove water level data from CSV
2. Explore environmental patterns and correlations
3. Analyze risk factors influencing flood events
4. Generate insights for coastal management

## Key Insights

- Environmental factors show strong correlation with water level risks
- Seasonal variations significantly impact flood probability
- Mangrove cover percentage inversely relates to flood risk
- Urban proximity affects hydrological patterns

## Future Enhancements

- Develop predictive ML models (Random Forest, XGBoost)
- Time series forecasting for water level prediction
- Geospatial visualization and mapping
- Integration with real-time monitoring systems

## Installation

To run this project locally:

```bash
# Clone the repository
git clone https://github.com/Krishna-v03/Mangrove-water-level-risk-project.git

# Install required packages
pip install pandas numpy matplotlib seaborn

# Open the Jupyter notebook
jupyter notebook Mangrove_water_level_risk_project.ipynb
