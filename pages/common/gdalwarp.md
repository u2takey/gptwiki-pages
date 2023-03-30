# gdalwarp 
## chatgpt 
The `gdalwarp` command is part of the GDAL (Geospatial Data Abstraction Library) software, which is used for translating, processing, and analyzing geospatial data. The command allows users to warp (or transform) raster datasets from one projection, resolution, or coordinate system to another. 

Here are some details about the `gdalwarp` command:

Syntax:

```
$ gdalwarp [options] source_file destination_file
```

Options:

- `-s_srs srs_def`: The source spatial reference system (SRS) in the format defined by the OGRSpatialReference class or a PROJ.4 string. 
- `-t_srs srs_def`: The target SRS in the same format as the source SRS. 
- `-r resampling_method`: The resampling method to use when reprojecting the raster, such as `near`, `bilinear`, `cubic`, or `average`. 
- `-tr xres yres`: Set the output resolution (in target georeferenced units per pixel) for both x and y directions. 
- `-te xmin ymin xmax ymax`: Set the output extent (in target georeferenced units) to the specified region. 
- `-dstnodata value`: Set nodata values to the specified value in the output file. 
- `-of format`: Set the output format to a specific format like GeoTIFF, JPEG, or PNG. 
- `-overwrite`: Overwrite the output file if it already exists. 

Examples:

```
$ gdalwarp -s_srs EPSG:4326 -t_srs EPSG:32612 input.tif output.tif
```

This command transforms a GeoTIFF raster from EPSG:4326 (WGS 84) to EPSG:32612 (WGS 84 / UTM zone 12N) projection.

```
$ gdalwarp -te 12.2 45.2 16.1 47.1 input.tif output.tif
```

This command clips a GeoTIFF file to a specified boundary in geographic coordinates.

Uses:

- Reprojecting raster datasets to different coordinate systems.
- Resampling or resizing raster datasets to a specific resolution.
- Clipping or merging raster datasets to create a new composite raster.
- Removing distortions from images caused by projections or resizing. 

Overall, `gdalwarp` is a powerful tool in the geospatial data processing industry and is widely used for a variety of applications. 

## tldr 
 
> Image reprojection and warping utility.
> More information: <https://gdal.org/programs/gdalwarp>.

- Reproject a raster dataset:

`gdalwarp -t_srs {{EPSG:4326}} {{path/to/input.tif}} {{path/to/output.tif}}`

- Crop a raster dataset by using specific coordinates:

`gdalwarp -te {{min_x}} {{min_y}} {{max_x}} {{max_y}} -te_srs {{EPSG:4326}} {{path/to/input.tif}} {{path/to/output.tif}}`

- Crop a raster dataset using a vector layer:

`gdalwarp -cutline {{path/to/area_to_cut.geojson}} -crop_to_cutline {{path/to/input.tif}} {{path/to/output.tif}}`
