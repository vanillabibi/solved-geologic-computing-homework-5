Download Link: https://assignmentchef.com/product/solved-geologic-computing-homework-5
<br>
<em>Please note</em>: Save your scripts to a directory named <em>Homework-5 </em>in your home account on the server computer in SCA 219 (131.247.211.166); do not email your answers. A short report should be typed and submitted in PDF format. A flowchart is not necessary for this assignment. Multiple pages should be stapled together. Some additional explanation is helpful and often necessary for the person reading your assignment to understand exactly what you are doing and why. Assume that the person grading your assignment does not have a copy of the assignment. What is important here is that <em>(1) </em>you understand what you are doing, and <em>(2) </em>that you can communicate what you are doing to others.

<h2>Introduction</h2>

In this homework assignment we begin to explore and create maps using Generic Mapping Tools (GMT). Be sure to read the handout about maps (maps.pdf) and the introduction to GMT (gmt.pdf) before trying to start this assignment. Work through the examples provided in these handouts.

In assignment 4, you calculated the volume of water in Crater Lake using a script and a data file, <em>filtered crater lake data.xyz</em>. Now look more carefully at the contents of this file. Each line of the file contains two geographic coordinates and an elevation. For example, the first line of the file shows:

568000 4758500 2041

The first two columns contain UTM coordinates of the elevation estimate. The last column is the elevation. Crater Lake is in UTM zone 10. The USGS saved the data using datum NAD27.

<h1>Problem 1</h1>

Use the Proj.4 Cartographic Library (see the maps.pdf handout) to convert this file from UTM coordinates to:

longitude latitude elevation

using the map <em>datum </em>WGS84. If you specify the name of your data file <em>(e.g., filtered crater lake data.xyz) </em>on the command line, after the parameter list, you can then redirect the conversions to a file using <em>&gt; filename</em>, the same syntax you used when executing your Perl or Python script. Note that when converting to longitudes and latitudes it is necessary to use <em>at least </em>6 decimal places, for accuracy.

For this problem, be sure to include in your report 1) the command line you use to make this file conversion and 2) the first 2 lines of your <em>converted </em>data file.

<h1>Problem 2</h1>

Now that you know the approximate latitude and longitude of Crater Lake:

Make a location map of the volcano using the GMT program <em>pscoast</em>. Be sure to include sufficient area so it is easy to visualize the location of the volcano with respect to geographic features of the western US (e.g., the coastline) and neaby US state boundaries.

Plot the location of Crater Lake on your location map and label it. Use the coordinate from Problem 1 and the GMT program <em>psxy </em>to plot the location of Crater Lake as a large red triangle. Label your red triangle using the GMT command <em>pstext</em>. Also label 2 US states, and any large, nearby bodies of water. This means you will have at least 4 pstext commands.

1

Explain the meaning of each GMT command and parameters used with each of your commands. Use the GMT manual pages, technical reference and cookbook, or the tutorial to find this information.

Report your results. The report should include 1) your problem statement(s), 2) a labeled location map, 3) a figure caption for your map which explains what and where and any symbols you used, 4)the GMT command lines that you used to create the map, and a description of what each GMT command comtributes to your map and how each parameter contributes to the command. Commands used multiple times only need to be described once.

2