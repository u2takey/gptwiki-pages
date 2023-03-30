# ogrinfo 
## chatgpt 
The "ogrinfo" command is a command-line tool used for working with spatial data in various vector formats.

The utility is part of the GDAL (Geospatial Data Abstraction Library) toolset and can be used to gather basic information about specific datasets such as shapefiles, GeoJSON, KML, or others.

Typically, the command is used to get an overview of the attributes and coordinate system of a data source, including the geometry that comprises the data. It can also be used to query specific information, including the number of features found in a particular dataset, as well as the spatial extent.

Some of the options that can be used with ogrinfo include:

-layers: lists the available layers in the chosen data source
-geom=SUMMARY: summarises the data geometry in the data source (points, lines, polygons etc)
-so: lists the open option strings for a specific data source

In summary, ogrinfo is an effective command-line tool for spatial data analysis, providing access to basic information about vector data sources in a wide range of formats. 

## tldr 
 
> List information about an OGR-supported data source.
> More information: <https://gdal.org/programs/ogrinfo.html>.

- List supported formats:

`ogrinfo --formats`

- List layers of a data source:

`ogrinfo {{path/to/input.gpkg}}`

- Get detailed information about a specific layer of a data source:

`ogrinfo {{path/to/input.gpkg}} {{layer_name}}`

- Show summary information about a specific layer of a data source:

`ogrinfo -so {{path/to/input.gpkg}} {{layer_name}}`

- Show summary of all layers of the data source:

`ogrinfo -so -al {{path/to/input.gpkg}}`

- Show detailed information of features matching a condition:

`ogrinfo -where '{{attribute_name > 42}}' {{path/to/input.gpkg}} {{layer_name}}`

- Update a layer in the data source with SQL:

`ogrinfo {{path/to/input.geojson}} -dialect SQLite -sql "{{UPDATE input SET attribute_name = 'foo'}}"`
