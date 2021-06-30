# global-earthquakes
Displays data of earthquakes around the world for the past month on a world map.

# Prerequisites to run the program:
- Make sure you have installed python, plotly, and json python library
- Download the json file from U.S. Geological Survey website: https://www.usgs.gov/
- Specifically this json file: https://earthquake.usgs.gov/earthquakes/feed/v1.0/summary/significant_month.geojson
- Rename it to a shorter filename

# How the program works:
- Opens the json file and load it as a python dictionary
- Filter the dictionary to get the value of the magnitudes, longitudes, latitudes, etc. of earthquakes that occured this past month
- Create a data structure to map the details of each earthquake
- Use plotly to plot the data onto a world map with Scatetrgeo
- Saves the plot as an html to render it on to the browser

# How to run and edit the python program
- Open eq_world_map.py with a text editor
- Change the filename variable to the directory where the json file is located
- Find offline.plot(fig, filename='global_earthquakes.html'); then change the attribute of the filename to whatever name you want as long as it is an html file
- Run the program
