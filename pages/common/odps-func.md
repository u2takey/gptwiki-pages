# odps func 
## chatgpt 
As an AI language model, I do not have access to the specific context you are referring to. Therefore, I am giving a general explanation of the "odps func" command. 

The "odps func" command is a command-line interface (CLI) command used in Alibaba Cloud MaxCompute (formerly known as ODPS), a big data processing platform. It is used to perform operations related to MaxCompute functions. MaxCompute functions are user-defined functions (UDFs) that can be used in MaxCompute SQL queries to perform custom data processing tasks.

With the "odps func" command, MaxCompute users can perform tasks such as creating, listing, updating, or deleting MaxCompute functions. The command takes various arguments and options to specify the action to be performed and the parameters required for the action.

To learn more about the "odps func" command and its usage, you can refer to the MaxCompute documentation or seek help from Alibaba Cloud MaxCompute support team. 

## tldr 
 
> Manage functions in ODPS (Open Data Processing Service).
> See also `odps`.
> More information: <https://www.alibabacloud.com/help/doc-detail/27971.htm>.

- Show functions in the current project:

`list functions;`

- Create a Java function using a `.jar` resource:

`create function {{func_name}} as {{path.to.package.Func}} using '{{package.jar}}';`

- Create a Python function using a `.py` resource:

`create function {{func_name}} as {{script.Func}} using '{{script.py}}';`

- Delete a function:

`drop function {{func_name}};`
