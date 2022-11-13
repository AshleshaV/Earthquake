# Earthquake


## Project Overview
The main objective is to gather earthquake GeoJSON data from the USGS API, create and explore interactive maps of earthquakes around the world.\
The earthquake data is represented on the maps in relation to the tectonic plates’ location on the earth, and according to each event's magnitude.



### Project Purpose
The purpose of this project is to visually show the differences between the magnitudes of earthquakes all over the world for the last seven days.

### Tasks
To complete this project, we use a URL for GeoJSON earthquake data from the [USGS website](https://www.usgs.gov/natural-hazards/earthquake-hazards/earthquakes) and retrieve geographical coordinates and the magnitudes of earthquakes for the last seven days. Then add the data to a map.









### Results:

## Creating the overlays and controls:

![image](https://user-images.githubusercontent.com/108908214/201509938-2e62443d-84c4-4337-bd48-d2e0521d9699.png)



## A light map layer with all earthquake toggles:
![image](https://user-images.githubusercontent.com/108908214/201509984-0841385f-4e83-4852-8c6d-a4268a5d87ec.png)

## A dark map layer with major earthquakes only:
![image](https://user-images.githubusercontent.com/108908214/201509991-e27a2b43-8d0d-41bf-9927-1a0241dc307d.png)

## Satellite streets layer with tectonic plates only:
![image](https://user-images.githubusercontent.com/108908214/201510000-76d78df1-be20-4ae8-b9f5-11c5e415b855.png)

## Streets layer with earthquakes only:
![image](https://user-images.githubusercontent.com/108908214/201510016-853bbe09-88bb-48d5-bfe9-aecfd1fdc971.png)



## Summary
Using the JavaScript and the D3.js library, [GeoJSON data](https://earthquake.usgs.gov/earthquakes/feed/v1.0/summary/all_week.geojson) we created the maps to retrieve the coordinates and magnitudes of the earthquakes.

Calling the API's alllowed us to traverse and retrieve [GeoJSON earthquake data](https://earthquake.usgs.gov/earthquakes/feed/v1.0/summary/all_week.geojson) and [tectonic plate data](https://raw.githubusercontent.com/fraxen/tectonicplates/master/GeoJSON/PB2002_boundaries.json) in order to populate a map. Later we used the [Leaflet library](https://leafletjs.com/index.html) to plot the data on a Mapbox map through an API request and create interactivity for the earthquake data. The viewer can toggle between different layers to view either all earthquakes, only major earthquakes (over 4.5 magnitude), and the earth's tectonic plates. 

By viewing this visualization, it's clear that the majority of the major earthquakes in the last week have all occurred near or on the tectonic plates. Smaller earthquakes can occur farther away, but the major earthquakes all fall on or right next to the fault lines. 
