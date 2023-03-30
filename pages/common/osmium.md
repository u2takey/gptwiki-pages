# osmium 
## chatgpt 
Osmium is a command-line tool used for various tasks related to OpenStreetMap (OSM) data. It is a part of the Osmium Tool suite, which is a collection of command-line tools for working with OSM data. 

The Osmium command provides various functions, including:

- Reading OSM data from a file or a URL and storing it in different formats such as PBF, XML, and JSON.
- Filtering and transforming OSM data using several criteria like node/way/relation types, tags, areas, and bounding boxes.
- Converting OSM data to different formats like CSV, GeoJSON, Shapefiles, and PostgreSQL.
- Editing OSM data and applying changes to an OSM database using Osmium Diff or Osmium Apply.
- Performing various data analysis tasks, such as counting nodes, ways, relations, and performing geometric operations like area calculation, convex hull, and centroid.

Overall, the Osmium command is a very powerful and flexible tool for working with OSM data, and it can be used for a wide range of data-processing tasks. Its extensive documentation and active development community make it an excellent resource for anyone working with OSM data. 

## tldr 
 
> Multipurpose tool for handling OpenStreetMap (OSM) files.
> More information: <https://osmcode.org/osmium-tool/manual>.

- Show file information:

`osmium fileinfo {{path/to/input.osm}}`

- Display contents:

`osmium show {{path/to/input.osm}}`

- Convert file format from PBF into XML:

`osmium cat {{path/to/input.osm.pbf}} -o {{path/to/output.osm}}`

- Extract a geographic region by the given [b]ounding box:

`osmium extract -b {{min_longitude}},{{min_latitude}},{{max_longitude}},{{max_latitude}} {{path/to/input.pbf}} -o {{path/to/output.pbf}}`

- Extract a geographic region by a GeoJSON file:

`osmium extract -p {{path/to/polygon.geojson}} {{path/to/input.pbf}} -o {{path/to/output.pbf}}`

- Filter all objects tagged as "restaurant":

`osmium tags-filter {{path/to/input.pbf}} amenity=restaurant -o {{path/to/output.pbf}}`

- Filter for "way" objects tagged as "highway":

`osmium tags-filter {{path/to/input.pbf}} w/highway -o {{path/to/output.pbf}}`

- Filter "way" and "relation" objects tagged as "building":

`osmium tags-filter {{path/to/input.pbf}} wr/building -o {{path/to/output.pbf}}`
