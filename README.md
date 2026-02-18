A Python tool that automates the generation of 3D city models using OpenStreetMap (OSM) data. This script extracts building footprints and street networks, extrudes them into 3D meshes, and allows for interactive visualization and export.

Key capabilities include:

Data Extraction: Fetches buildings and street networks from OSM using osmnx.

3D Extrusion: Generates 3D meshes by vertically extruding building footprints.

Height Handling: Automatically assigns random heights (35m–50m) to buildings that lack height tags in OSM.

Visualization: Renders the city interactively using PyVista.

Export: Saves the resulting 3D models as .obj files for use in other 3D software (Blender, Unity, etc.).

Animation: Optionally generates a rotating GIF animation of the generated city.

🚀 Features

Automated Workflow: From data fetch to 3D model in a single script.

Street Network Integration: Converts 2D street lines into 3D tubes for better visualization.

Interactive Viewer: Inspect the model directly in Python.

Portable Output: Exports standard .obj meshes to the Output/ directory.

🛠️ Prerequisites
To run this script, you need Python installed along with the following libraries:

osmnx (for OSM data retrieval)

pyvista (for 3D plotting and mesh generation)

geopandas (for handling geospatial data frames)

numpy (for numerical operations)

⚠️ Important Notes

Coordinate Systems (CRS): The script handles CRS transformations, but ensure any external datasets you integrate use a consistent EPSG code to avoid misalignment.

Building Heights: OpenStreetMap often lacks height data for every building. This script handles missing values by assigning a random height between 35 and 50 units. For accurate heights, you would need to integrate LiDAR or DTM data.


All of the DTM and LiDAR data for Australia can be found on https://elevation.fsdf.org.au/



Almost all of this was made with the help of the tutorial videos from Dr.Florent Poux
