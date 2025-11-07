# 3d_city_modeling
This script generates a 3D model and gif of Sydney (or any other city).

Extracts OSM data (buildings, streets) for a specified location and radius.
Generates building footprints and assigns heights.
Extrudes buildings vertically to create 3D meshes.
Visualization & Export
Convert streets to 3D lines
Displays the model interactively in PyVista (pl.show()), or
Saves the meshes as .obj files under Output/<City>/.

Optionally, cloudgify() generates a rotating GIF animation of the model.

Important warnings
EPSG code mismatch
Make sure all datasets use the same coordinate reference system (CRS).

Building height handling
Not all OSM buildings include the height data, therefore height was set to random(35,50)




Almost all of this was made with the help of the tutorial videos from Dr.Florent Poux
