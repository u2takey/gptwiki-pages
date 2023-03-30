# ogrmerge.py 
## chatgpt 
`ogrmerge.py` is a command-line tool for merging multiple OGR-supported vector datasets into a single output file. 

OGR (OpenGIS Simple Features Reference Implementation) is a library for reading and writing vector data formats such as shapefiles, GeoJSON, KML, and many others. It provides a consistent interface for accessing vector data across formats and can be used with many GIS software packages.

The `ogrmerge.py` command takes the following syntax:

```
ogrmerge.py [-o out_filename] [-single] [-overwrite] [-progress] [-f format] [input_files]
```

- `-o out_filename`: specifies the filename for the output file. If not specified, the merged file is written to standard output.
- `-single`: creates a single output layer by merging all input layers. By default, input layers are preserved as separate layers in the output file.
- `-overwrite`: allows the output file to overwrite existing files.
- `-progress`: displays a progress bar during processing.
- `-f format`: specifies the output format. If not specified, the output format is inferred from the output filename.
- `input_files`: a list of one or more input datasets to be merged. Each input dataset should include the format specifier, such as `-f ESRI Shapefile`. 

For example, the following command would merge two shapefiles (`input1.shp` and `input2.shp`) into a single output file (`output.shp`) in ESRI Shapefile format:

```
ogrmerge.py -o output.shp -single input1.shp input2.shp
``` 

## tldr 
 
> Merge several vector datasets into a single one.
> More information: <https://gdal.org/programs/ogrmerge.html>.

- Create a GeoPackage with a layer for each input Shapefile:

`ogrmerge.py -f {{GPKG}} -o {{path/to/output.gpkg}} {{path/to/input1.shp path/to/input2.shp ...}}`

- Create a virtual datasource (VRT) with a layer for each input GeoJSON:

`ogrmerge.py -f {{VRT}} -o {{path/to/output.vrt}} {{path/to/input1.geojson path/to/input2.geojson ...}}`

- Concatenate two vector datasets and store source name of dataset in attribute 'source_name':

`ogrmerge.py -single -f {{GeoJSON}} -o {{path/to/output.geojson}} -src_layer_field_name country {{source_name}} {{path/to/input1.shp path/to/input2.shp ...}}`
