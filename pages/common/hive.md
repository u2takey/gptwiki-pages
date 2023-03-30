# hive 
## chatgpt 
The command "hive" is used to start the Apache Hive service, which is a data warehouse infrastructure built on top of Hadoop. It allows users to easily query and analyze large datasets stored in Hadoop Distributed File System (HDFS) using a SQL-like language called HiveQL. 

When the "hive" command is executed, it starts the Hive shell, which is a command-line interface that allows users to execute HiveQL commands and interact with the Hive metastore. The Hive metastore is a database that stores metadata about the datasets and the tables created in Hive, as well as the associated schema and other information required to process and analyze the data efficiently.

Once the Hive shell is started, users can define tables, load data into them, and query the data using HiveQL commands. Hive provides a rich set of built-in functions and operators that can be used to perform various types of data transformations, filtering, sorting, and aggregation operations.

In summary, the "hive" command is the starting point for using the Apache Hive data warehouse infrastructure, providing users with a powerful tool for querying and analyzing large datasets stored in Hadoop. 

## tldr 
 
> CLI tool for Apache Hive.
> More information: <https://cwiki.apache.org/confluence/display/Hive/LanguageManual+Cli>.

- Start a Hive interactive shell:

`hive`

- Run HiveQL:

`hive -e "{{hiveql_query}}"`

- Run a HiveQL file with a variable substitution:

`hive --define {{key}}={{value}} -f {{path/to/file.sql}}`

- Run a HiveQL with HiveConfig (e.g. `mapred.reduce.tasks=32`):

`hive --hiveconf {{conf_name}}={{conf_value}}`
