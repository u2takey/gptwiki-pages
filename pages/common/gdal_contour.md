# gdal_contour 
## chatgpt 
The "gdal_contour" command is a tool that is part of the open-source Geospatial Data Abstraction Library (GDAL). This tool is used to create contour lines from elevation raster data.

Here's a breakdown of the command:

- "gdal_contour" is the name of the command.
- The command takes several arguments, including the input raster file (which contains the elevation data) and the output vector file (which will contain the contour lines).
- The "-a" option specifies which attribute should be used to label the contour lines. By default, the command uses the value of the elevation raster as the attribute.
- The "-i" option specifies the interval between contour lines. For example, setting "-i 10" would create contour lines every 10 units of elevation.
- The "-snodata" option specifies the value in the input raster that represents "no data". This value will be ignored when creating the contour lines.

Overall, the "gdal_contour" command is a powerful tool for creating high-quality contour lines from elevation data. By adjusting the various options, you can customize the output to suit your needs. 

## tldr 
 
> Create contour lines and polygons from a digital elevation model.
> More information: <https://gdal.org/programs/gdal_contour.html>.

- Create a vector dataset with contour lines spread over an 100-meter [i]nterval while [a]ttributing the elevation property as "ele":

`gdal_contour -a {{ele}} -i {{100.0}} {{path/to/input.tif}} {{path/to/output.gpkg}}`

- Create a vector dataset with [p]olygons spread over an 100-meter [i]nterval:

`gdal_contour -i {{100.0}} -p {{path/to/input.tif}} {{path/to/output.gpkg}}`
