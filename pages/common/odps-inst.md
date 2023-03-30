# odps inst 
## chatgpt 
As an AI language model, I assume that you are referring to the Alibaba Cloud command "odps inst". 

The "odps inst" command is used in Alibaba Cloud's MaxCompute service to manage the life cycle of a specific instance of a job. With this command, users can query, stop or restart a running job instance.

Here are the subcommands that can be used with "odps inst":

1. "odps inst query" - This subcommand is used to query the status and details of a specific job instance by providing the name, task name, and instanceID.

2. "odps inst kill" - This subcommand is used to stop a running job instance by providing the name, task name, and instanceID.

3. "odps inst restart" - This subcommand is used to restart a failed job instance by providing the name, task name, and instanceID.

In summary, "odps inst" is a command that helps users manage the instances of specific jobs in their MaxCompute clusters, which can be useful for monitoring and troubleshooting purposes. 

## tldr 
 
> Manage instances in ODPS (Open Data Processing Service).
> See also `odps`.
> More information: <https://www.alibabacloud.com/help/doc-detail/27971.htm>.

- Show instances created by current user:

`show instances;`

- Describe the details of an instance:

`desc instance {{instance_id}};`

- Check the status of an instance:

`status {{instance_id}};`

- Wait on the termination of an instance, printing log and progress information until then:

`wait {{instance_id}};`

- Kill an instance:

`kill {{instance_id}};`
