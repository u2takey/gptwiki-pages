# gdalbuildvrt 
## chatgpt 
The "gdalbuildvrt" command is a tool in the GDAL (Geospatial Data Abstraction Library) library used to create a virtual raster file from a group of other raster files. The virtual raster file doesn't contain actual raster data but stores metadata about these raster files. The command has the following syntax:

gdalbuildvrt [options] output_file input_files...

Where:
- "[options]" are the additional settings for the command. Some of the available options are:
    - "-separate": stores each band of the input files as a separate layer in the output file.
    - "-resolution {highest/lowest/average}": sets the resolution for the output file, based on either the highest, lowest or average resolution of input files.
    - "-te xmin ymin xmax ymax": sets the geospatial extent for the output file in the format "xmin ymin xmax ymax".
- "[output_file]" is the name and location of the output file.
- "[input_files...]" is the list of input raster files that will be used to create the virtual raster file.

The "gdalbuildvrt" command is often used to mosaic or merge multiple raster files into a single file, making it easier to manage and display large amounts of data. It can also be used to create an overview pyramid or a reduced resolution version of the output file, improving its visualization performance. 

## tldr 
 
> Build Virtual Datasets from a list of existing datasets.
> More information: <https://gdal.org/programs/gdalbuildvrt.html>.

- Make a virtual mosaic from all TIFF files contained in a directory:

`gdalbuildvrt {{path/to/output.vrt}} {{path/to/input_directory/*.tif}}`

- Make a virtual mosaic from files whose name is specified in a text file:

`gdalbuildvrt -input_file_list {{path/to/list.txt}} {{path/to/output.vrt}}`

- Make an RGB virtual mosaic from 3 single-band input files:

`gdalbuildvrt -separate {{path/to/rgb.vrt}} {{path/to/red.tif}} {{path/to/green.tif}} {{path/to/blue.tif}}`

- Make a virtual mosaic with blue background color (RGB: 0 0 255):

`gdalbuildvrt -hidenodata -vrtnodata "{{0 0 255}}" {{path/to/output.vrt}} {{path/to/input_directory/*.tif}}`
