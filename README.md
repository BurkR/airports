# airports
lab3
5. Deliverable
After you successfully deploy this cell tower map, you are expected to build another web map of airports in United States. In the assets directory of this lab, you will see two geojson files: one is airports.geojson, another is us-states.geojson.
=========================================================================================================================
OK, I got the cell tower map to display in Chrome. I made a screen shot of this called: cellphonetowers_screenshot.jpg and placed it in this directory.  

The project name is a scaleable map entitled: "Airports of the United States".

Two map layers were used including a United States base map and a map of airports across the United States. One of the fields in the airport layer was control towers, named: CTRL_TRS. This field was used to indicate whether the airport had a control tower or not. Therefore a Javascript function was added, within MapBox layer panel, to indicate the presence of a tower on the map with a "Y" for yes and a "N" for no.

Methods for this project include: The map projection was updated to CRS: WGS-84 projection using QGIS. The file was added to QGIS as a layer then Under the layer properties the projection was changed as well as a few other attributes to make the U.S. Layer compatible with a web environment. The number of digits in the coordinates was reduced from 15 characters to 10 characters to make the data load efficiently on the webpage. In order to reduce the map coverage further, the map files were opened in mapshaper.org. After simplifying the code in mapshaper.org the files were uploaded to MapBox for making the final display edits.

The source of united states base map and the distribution of airports came from Professor Zhao, who downloaded the maps from Mike Bostock of D3 in the form of geojson files. The map elements were combined in MapBox including the color scheme and the icons were created with the help of all maki icons. The completed map was published using the MapBox provided code, that was pasted into the Github index file. Several versions of this code were saved on the local labtop hard drive to control for errors. Github was used to display the final map webpage in the Index file, seen at the following URL: https://burkr.github.io/maps/.

[airports]
    │index.html
    │readme.md
    ├─assets
    │      airports.geojson
    │      us-states.geojson
    ├─css
    │      main.css
    ├─img
    │      xxx.jpg
    └─js
            main.js

===================================================================================================================

airports.geojson contains all the airports in United States. This data is converted from a shapefile, which was downloaded and unzipped from https://catalog.data.gov/dataset/usgs-small-scale-dataset-airports-of-the-united-states-201207-shapefile. For each airport feature, the field CNTL_TWR indicates whether the airport has an air traffic control tower or not. If there is a tower, the value of CNTL_TWR is 'Y', otherwise 'N'. You may need to find an appropriate icon on font awesome. (7 points)

us-states.geojson is a geojson data file containing all the states boundaries of United States. This data is acquired from from Mike Bostock of D3. The count field indicates the number of airports within the boundary of the state under investigation. So please make a choropleth map based on the number of airports within each state. (7 points)

an appropriate basemap; (7 points)

some interactive elements, like a clickable marker; (8 points)

some map elements, such as legend, scale bar, credit; (8 points)

write up a project description in the readme.md file. This file will introduce the project name, a brief introduction, the major functions(especially the function which was not covered in the lectures), libraries, data sources, credit, acknowledgement, and other necessary information. (8 points)

you will need to synchronize this project to a github repository. And make sure the web map is accessible from a url link, which should be similar to http://[your_github_username].github.io/[your_repository_name]/index.html. (To do that, you may want to check out previous lecture or lab handouts on how to host repository on github pages.); (6 points)

Note: Please make sure the name of your repository is NOT lab03 or similiar, use a name which can describe the theme of the map you will make. Think about that, which one do you prefer? - showing your future employer or Ph.D. admission committee a lot of course work on github or a list of professional projects.

please make sure the internal structure of the files in your project repository is well organized. For example, it may be similar to the file structure below. (5 points)
Optional tasks:
Try to add on a feature of leaflet which we have not discussed in class. The new features can be found on the plugin page of leafet; (5 points)
If you have a genuine reason(known medical condition, a pile-up of due assignments on other courses, ROTC,athletics teams, job interview, religious obligations etc.) for being unable to complete work on time, then some flexibility is possible. However, if in my judgment you could reasonably have let me know beforehand that there would likely be a delay, and then a late penalty will still be imposed if I don't hear from you until after the deadline has passed. For unforeseeable problems,I can be more flexible. If there are ongoing medical, personal, or other issues that are likely to affect your work all semester, then please arrange to see me to discuss the situation. There will be NO make-up exams except for circumstances like those above.
