# Satellite-Based Monitoring System for Land Use and Land Cover Changes for Sustainable Development 🌍

![image](https://github.com/user-attachments/assets/e5472acb-2c8c-4dfa-a4dd-71555b2c6a63)

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [How It Works](#Application Workflow)
- [Usage](#usage)
- [Folder Structure](#folder-structure)
- [Dataset](#dataset)
- [Installation](#installation)
- [How to Run](#how-to-run)
- [Demo](#demo)
- [Team](#team)
- [License](#license)
- [Acknowledgements](#acknowledgements)
## Introduction
This repository contains an AI-based platform designed to classify **Land Use and Land Cover (LULC)** from **Sentinel-2 satellite imagery**. The platform is developed as part of the [Hack4Earth Hackathon](https://hack4earth.org), focusing on sustainable environmental solutions through AI. OptiLand-Ai is an AI-powered web application for LULC prediction using satellite imagery. The app allows users to select a province, view satellite imagery, and predict LULC classes, while also calculating the CO₂ impact based on different land covers. This tool is particularly useful for environmental monitoring and sustainability analysis.

## Features
- **LULC Prediction**: Uses a pre-trained ResNet50 model to predict different LULC classes such as forests, residential areas, industrial areas, and more.
- **Satellite Image Visualization**: Displays the satellite imagery of selected provinces with overlaid predictions using Folium.
- **CO₂ Impact Calculation**: Estimates the total CO₂ impact based on the predicted land use classes.
- **Interactive Map**: Integrates Folium and Streamlit for an interactive experience, including map layers and LULC class legends.
- **Class Distribution**: Displays a bar chart of the distribution of predicted LULC classes with a breakdown of their CO₂ impact.

### Application Workflow:
1. **Select a Province**: Use the sidebar to select one of the available provinces (e.g., Tunis, Monastir).
2. **View Satellite Imagery**: The app will load and display satellite images for the selected province.
3. **LULC Prediction**: The app will automatically generate grid tiles over the selected region and predict LULC classes for each tile.
4. **CO₂ Calculation**: Optionally, click the Calculate CO₂ button to estimate the CO₂ impact of the predicted land classes.

### LULC Classes and CO₂ Impact Rates
| LULC Class              | Color          | CO₂ Impact (tons) |
|------------------------|----------------|--------------------|
| AnnualCrop             | Light Green    | 2.5                |
| Forest                 | Forest Green   | -20                |
| HerbaceousVegetation    | Yellow Green   | -5                 |
| Highway                | Gray           | 10                 |
| Industrial             | Red            | 50                 |
| Pasture                | Medium Sea Green| 1.5               |
| PermanentCrop          | Chartreuse     | -3                 |
| Residential            | Magenta        | 15                 |
| River                  | Dodger Blue    | 0                  |
| SeaLake                | Blue           | 0                  |

## Technologies Used
- **Streamlit**: For creating the web interface.
- **PyTorch**: For loading and running the pre-trained ResNet50 model.
- **Earth Engine (EE)**: For initializing and processing satellite imagery.
- **Geopandas & Rasterio**: For working with geospatial data and raster images.
- **Folium**: For map visualization.
- **Plotly**: For generating interactive plots and charts.


### Demo
[Watch video](assets/LUCD.mp4)



### Clone the Repository
- **git clone**:https://github.com/FadwaHarrabi/Hack4Earth-OptiLand-Ai.git

### Install Requirements
Install all the dependencies required to run the app:
- pip install -r requirements.txt

### Usage
To run the Streamlit app, execute the following command:
- streamlit run app.py
## Team
the team leader:Wadie Kadri
Team member :Fadwa Harrabi
## License
This project is licensed under the MIT License.

## Acknowledgements
- Google Earth Engine for providing satellite data.
- PyTorch for the deep learning framework.
- Streamlit for simplifying web app development.

For more details check the authors profile
- Kadri WADIE[](https://www.linkedin.com/in/kadri-wadie?lipi=urn%3Ali%3Apage%3Ad_flagship3_profile_view_base_contact_details%3BfMVI6fNCQxmvDpQs993TCg%3D%3D)
- Fadwa Harrabi (https://www.linkedin.com/in/fadwa-harrabi-546746259?lipi=urn%3Ali%3Apage%3Ad_flagship3_profile_view_base_contact_details%3BjyZm9EJlTUyR6%2FB2xhEzBg%3D%3D)
