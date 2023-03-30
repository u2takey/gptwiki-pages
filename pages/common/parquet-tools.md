# parquet-tools 
## chatgpt 
Parquet-tools is a command-line tool used to inspect, debug, and analyze Parquet files. Parquet is a columnar storage format that is specifically designed for use in distributed computing environments, such as Hadoop, Spark, and Hive. The tool provides several commands to work with Parquet files, including:

1. `cat`: This command displays the contents of a Parquet file in plain text format.
2. `meta`: This command displays the metadata of a Parquet file, including the schema and column statistics.
3. `head`: This command displays the first few rows of a Parquet file.
4. `schema`: This command displays the schema of a Parquet file in JSON format.
5. `validate`: This command validates the integrity of a Parquet file.

These commands can be useful for debugging and analyzing Parquet files, as well as for understanding the data stored within them. Additionally, Parquet-tools can be used in conjunction with other tools, such as Hive or Spark, to perform more advanced analysis and processing of Parquet files. 

## tldr 
 
> A tool to show, inspect and manipulate Parquet file.
> More information: <https://github.com/apache/parquet-mr/tree/master/parquet-tools-deprecated>.

- Display the content of a Parquet file:

`parquet-tools cat {{path/to/parquet}}`

- Display the first few lines of a Parquet file:

`parquet-tools head {{path/to/parquet}}`

- Print the schema of a Parquet file:

`parquet-tools schema {{path/to/parquet}}`

- Print the metadata of a Parquet file:

`parquet-tools meta {{path/to/parquet}}`

- Print the content and metadata of a Parquet file:

`parquet-tools dump {{path/to/parquet}}`

- Concatenate several Parquet files into the target one:

`parquet-tools merge {{path/to/parquet1}} {{path/to/parquet2}} {{path/to/target_parquet}}`

- Print the count of rows in a Parquet file:

`parquet-tools rowcount {{path/to/parquet}}`

- Print the column and offset indexes of a Parquet file:

`parquet-tools column-index {{path/to/parquet}}`
