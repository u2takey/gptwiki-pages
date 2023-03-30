# odps tunnel 
## chatgpt 
The command "odps tunnel" is used in Alibaba Cloud's MaxCompute service to create a secure tunnel between a local machine and a MaxCompute project, allowing data to be transferred securely between the two.

The command has several subcommands that allow different configurations and functionality, such as:

1. "create" - creates a new secure tunnel between the local machine and a MaxCompute project.
2. "list" - lists all the active tunnels currently running.
3. "kill" - shuts down an active tunnel.
4. "start" - starts an existing tunnel that was previously stopped.
5. "stop" - stops an active tunnel.
6. "status" - shows the current status of an active tunnel.

When creating a new secure tunnel, the user needs to specify the local and remote ports to use for the connection, as well as the MaxCompute project they want to connect to. The command also requires authentication credentials, such as an AccessKey ID and Secret, to ensure secure communication between the local machine and the MaxCompute project.

Once the tunnel is established, the local machine can securely access the data stored in the MaxCompute project as if it were on the local machine. This is useful for data analysis and processing tasks that require access to large datasets that may be too large to transfer over the internet in a timely manner. 

## tldr 
 
> Data tunnel in ODPS (Open Data Processing Service).
> See also `odps`.
> More information: <https://www.alibabacloud.com/help/doc-detail/27971.htm>.

- Download table to local file:

`tunnel download {{table_name}} {{path/to/file}};`

- Upload local file to a table partition:

`tunnel upload {{path/to/file}} {{table_name}}/{{partition_spec}};`

- Upload table specifying field and record delimiters:

`tunnel upload {{path/to/file}} {{table_name}} -fd {{field_delim}} -rd {{record_delim}};`

- Upload table using multiple threads:

`tunnel upload {{path/to/file}} {{table_name}} -threads {{num}};`
