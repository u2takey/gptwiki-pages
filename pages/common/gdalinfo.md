# gdalinfo 
## chatgpt 
`gdalinfo` is a command-line tool that is part of the Geospatial Data Abstraction Library (GDAL). It provides information about a raster or vector dataset, including information about its metadata, projection, and dimensions.

Here is the breakdown of the command:

- `gdalinfo`: This is the command name that needs to be entered in the command-line interface to use the tool.
- `<dataset_name>`: This argument specifies the name and location of the dataset that the user wants to get information about. The dataset can be in various formats (e.g., GeoTIFF, NetCDF, Shapefile).
- `-stats`: This optional argument calculates statistics for the data in the dataset, including the minimum, maximum, mean, and standard deviation. These statistics are printed out along with the other dataset information.
- `-hist`: This optional argument generates a histogram of the data in the dataset, showing the distribution of pixel values. The histogram is printed out along with the other dataset information.
- `-nogcp`: This optional argument prevents the printing of any ground control points (GCPs) that may be included in the dataset's metadata. By default, GCPs are printed if they exist in the dataset.

Once the command is entered, `gdalinfo` reads the metadata of the dataset and displays information about it. This information includes:

- The dataset format
- The size and dimensions of the dataset
- The number of bands in the dataset
- The pixel datatype
- The projection information (if available)
- The metadata associated with the dataset (if available)
- The calculated statistics (if `-stats` is used)
- The histogram (if `-hist` is used)
- Any ground control points (if `-nogcp` is not used) 

## tldr 
 
> List various information about a GDAL supported raster dataset.
> More information: <https://gdal.org/programs/gdalinfo.html>.

- List all supported raster formats:

`gdalinfo --formats`

- List information about a specific raster dataset:

`gdalinfo {{path/to/input.tif}}`

- List information about a specific raster dataset in JSON format:

`gdalinfo -json {{path/to/input.tif}}`

- Show histogram values of a specific raster dataset:

`gdalinfo -hist {{path/to/input.tif}}`

- List information about a Web Map Service (WMS):

`gdalinfo WMS:{{https://services.meggsimum.de/geoserver/ows}}`

- List information about a specific dataset of a Web Map Service (WMS):

`gdalinfo WMS:{{https://services.meggsimum.de/geoserver/ows}} -sd {{4}}`
