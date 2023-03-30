# ogr2ogr 
## chatgpt 
ogr2ogr is a command-line utility that allows users to convert and manipulate geospatial data between various formats, such as shapefiles, GeoJSON, KML, and PostGIS. It is a part of the GDAL (Geospatial Data Abstraction Library) open-source software suite.

The basic syntax of the ogr2ogr command is as follows:

```
ogr2ogr [options] destination_data_source input_data_source
```

- `options`: These are optional command-line flags that modify the behavior of ogr2ogr. Some commonly used options include `-f` for specifying the output format, `-s_srs` and `-t_srs` for specifying the source and target coordinate reference systems, `-sql` for executing SQL commands on the input data, and many others. See the ogr2ogr documentation for a complete list.

- `destination_data_source`: This is the output file or data store where the converted data will be written to. The data source can be a file path, a URL (if the output format supports it), or a connection string to a database.

- `input_data_source`: This is the source data that will be converted. It can be a file path, a URL, or a connection string to a database.

Here are some examples of how the ogr2ogr command can be used:

```
# Convert a shapefile to GeoJSON
ogr2ogr -f GeoJSON output.geojson input.shp

# Convert a KML file to a CSV file
ogr2ogr -f CSV output.csv input.kml

# Import a CSV file into a PostgreSQL database
ogr2ogr -f PostgreSQL PG:"dbname=mydatabase" input.csv

# Export a PostGIS table to a GeoJSON file
ogr2ogr -f GeoJSON output.geojson PG:"dbname=mydatabase" -sql "SELECT * FROM mytable"
```

Overall, ogr2ogr is a powerful and flexible tool for working with geospatial data, and its wide range of supported formats allows for easy integration with other GIS software and workflows. 

## tldr 
 
> Convert geospatial vector data between file formats.
> More information: <https://gdal.org/programs/ogr2ogr.html>.

- Convert a Shapefile into a GeoPackage:

`ogr2ogr -f GPKG {{path/to/output}}.gpkg {{path/to/input}}.shp`

- Reduce a GeoJSON to features matching a condition:

`ogr2ogr -where '{{myProperty > 42}}' -f {{GeoJSON}} {{path/to/output.geojson}} {{path/to/input.geojson}}`

- Change coordinate reference system of a GeoPackage from `EPSG:4326` to `EPSG:3857`:

`ogr2ogr -s_srs {{EPSG:4326}} -t_srs {{EPSG:3857}} -f GPKG {{path/to/output}}.gpkg {{path/to/input}}.gpkg`

- Convert a CSV file into a GeoPackage, specifying the names of the coordinate columns and assigning a coordinate reference system:

`ogr2ogr -f GPKG {{path/to/output}}.gpkg {{path/to/input}}.csv -oo X_POSSIBLE_NAMES={{longitude}} -oo Y_POSSIBLE_NAMES={{latitude}} -a_srs {{EPSG:4326}}`

- Load a GeoPackage into a PostGIS database:

`ogr2ogr -f PostgreSQL PG:dbname="{{database_name}}" {{path/to/input}}.gpkg`

- Clip layers of a GeoPackage file to the given bounding box:

`ogr2ogr -spat {{min_x}} {{min_y}} {{max_x}} {{max_y}} -f GPKG {{path/to/output}}.gpkg {{path/to/input}}.gpkg`
