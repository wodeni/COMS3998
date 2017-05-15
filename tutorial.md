# Conversion from ESRI Multipatch to FBX

## 1. Overview

In this tutorial, we will show the necessary step to convert from Esri Multipatch to a 3D Model that can be used in Unity 3D.

## 2. Prerequisites

Multiple softwares are required for this conversion:

- ArcGIS 10.5: ArcMap and ArcScene are used.
- Blender
- CityEngine

## 3. Retrieving the Model and Building footprints

A complete 3D model of all buildings in New York City are available at Department of Information Technologies and Telecommunication(DoITT)'s [offical website](http://www1.nyc.gov/site/doitt/initiatives/3d-building.page). In this tutorial we are going to use "Multipatch (ESRI)" format. Download the `.zip` file here: http://maps.nyc.gov/download/3dmodel/DA_WISE_Multipatch.zip. Unzip the file to the desired location.

This model consists of multiple parts divided in to "delivery areas". For the area that contains Columbia University campus, we use delivery area number `13`, which contains the Manhattan Island.

We will also need the building footprints from NYC OpenData's [official website](https://data.cityofnewyork.us/Housing-Development/Building-Footprints/nqwf-w8eh). Once the web page is loaded, click the "Export" button on the top right corner of the Map. Select "Shapefile" as the format. A `.zip` file will be automatically downloaded. Unzip the file to the desired location.

## 4. Conversion to VRML using ArcGIS

To properly import our Multipatch data, we will be using two softwares from Esri's ArcGIS software[1]: ArcMap and ArcScene. We will use ArcMap to import the original data, select the area of interest, and export in Shapefile format. We then use ArcScene to open the newly created Shapefile, and export the model to Virtual Reality Modeling Language(VRML) format[2], which is readable my many modeling softwares.

### Importing Multipatch data to ArcMap

1. Start up ArcMap, in the `File` menu on the toolbar, click `Add data`
2. In the file navigator, locate the upzipped DoITT model (TIDO)
3. Once imported successfully, you should be able to see a flattened version of the Manhattan Island.
4.


## 5. Conversion to FBX using Blender

Since VRML format is not directly supported by Unity, we have to further convert the product from the last step to FBX format. There are many possible choices of modeling softwares. In this tutorial, we will use Blender.

1. Open blender and create an empty Scene
2. Remove the cube in the center, the camera, the light, and the lamp.
3.

## 6. importing the model into Unity

## References

[1] ArcGIS Desktop official website, http://desktop.arcgis.com/en/.
[2] VRML Wikipedia page, https://en.wikipedia.org/wiki/VRML.
