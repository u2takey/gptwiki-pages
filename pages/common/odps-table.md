# odps table 
## chatgpt 
The command "odps table" is used to display information about a table in an Alibaba Cloud MaxCompute project. Here is a breakdown of the command:

- "odps" refers to the command-line interface of Alibaba Cloud MaxCompute, a big data processing and analytics platform.
- "table" is the keyword used to indicate that the command is related to displaying information about a table.

When executed, the "odps table" command displays the following information about a specific table:

- Table name: The name of the table being queried.
- Owner and Creation Time: The ID of the project or user who owns the table, and the time when it was created.
- Table partition keys: If the table is partitioned, this indicates the partition columns.
- Table Properties: Various configuration options for the table, such as the file format and storage location.
- Columns: The names and types of the columns in the table.

Overall, the "odps table" command is useful for obtaining important metadata about a table in an Alibaba Cloud MaxCompute project, which can help users better understand the data they are working with and optimize queries for better performance. 

## tldr 
 
> Create and modify tables in ODPS (Open Data Processing Service).
> See also `odps`.
> More information: <https://www.alibabacloud.com/help/doc-detail/27971.htm>.

- Create a table with partition and lifecycle:

`create table {{table_name}} ({{col}} {{type}}) partitioned by ({{col}} {{type}}) lifecycle {{days}};`

- Create a table based on the definition of another table:

`create table {{table_name}} like {{another_table}};`

- Add partition to a table:

`alter table {{table_name}} add partition ({{partition_spec}});`

- Delete partition from a table:

`alter table {{table_name}} drop partition ({{partition_spec}});`

- Delete table:

`drop table {{table_name}};`
