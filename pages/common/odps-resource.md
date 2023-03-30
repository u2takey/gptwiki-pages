# odps resource 
## chatgpt 
The `odps resource` command is used in Alibaba Cloud's MaxCompute (previously known as ODPS) platform to manage the resources used in a job or task.

Here is a breakdown of the different components of the command:

- `odps`: This refers to the command line tool that is used to interact with the MaxCompute platform.
- `resource`: This is one of the subcommands that can be used with the `odps` command. It is used to manage resources that are associated with a project.

Some of the actions that can be performed using the `odps resource` command include:

- Listing resources: You can use this command to list all the resources that are available in a project. This can help you to identify the resources that are currently in use and the ones that are not being used.
- Adding resources: You can use this command to add new resources to a project. This could include things like adding new jars or files that are needed for a particular job.
- Updating resources: If you need to make changes to the settings of a resource that is already in use, you can use this command to update it.
- Deleting resources: If you have resources that are no longer needed, you can use this command to delete them from the project.

Overall, the `odps resource` command is a useful tool for managing the resources associated with a MaxCompute project. By using this command, you can ensure that your jobs and tasks are running as efficiently as possible. 

## tldr 
 
> Manage resources in ODPS (Open Data Processing Service).
> See also `odps`.
> More information: <https://www.alibabacloud.com/help/doc-detail/27971.htm>.

- Show resources in the current project:

`list resources;`

- Add file resource:

`add file {{filename}} as {{alias}};`

- Add archive resource:

`add archive {{archive.tar.gz}} as {{alias}};`

- Add .jar resource:

`add jar {{package.jar}};`

- Add .py resource:

`add py {{script.py}};`

- Delete resource:

`drop resource {{resource_name}};`
