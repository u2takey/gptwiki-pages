# amass db 
## chatgpt 
The command "amass db" is used in the Amass tool, which is a reconnaissance tool for discovering targets on the internet. This command is used to manage the target data stored in the Amass database. 

When the "amass db" command is executed, it opens up a sub-menu with several different commands to interact with the database. Some of the common commands available in the "amass db" sub-menu are:

- "add" : This command is used to add new targets to the Amass database. The user can either add a single target manually or import a list of targets from a file.

- "show" : This command is used to display the target data stored in the Amass database. The user can view the targets that are currently in the database, or display various pieces of information about a specific target.

- "del" : This command is used to delete targets from the Amass database. The user can either delete a single target or delete multiple targets at once.

- "merge" : This command is used to merge two or more Amass databases together. The user can specify which databases to merge, and the resulting merged database will contain all of the targets from the original databases.

Overall, the "amass db" command is an important tool for managing the target data stored in the Amass database. It allows users to add targets, view target data, delete targets, and merge multiple databases together. 

## tldr 
 
> Interact with an Amass database.
> More information: <https://github.com/OWASP/Amass/blob/master/doc/user_guide.md#the-db-subcommand>.

- List all performed enumerations in the database:

`amass db -dir {{path/to/database_directory}} -list`

- Show results for a specified enumeration index and domain name:

`amass db -dir {{path/to/database_directory}} -d {{domain_name}} -enum {{index_from_list}} -show`

- List all found subdomains of a domain within an enumeration:

`amass db -dir {{path/to/database_directory}} -d {{domain_name}} -enum {{index_from_list}} -names`

- Show a summary of the found subdomains within an enumeration:

`amass db -dir {{path/to/database_directory}} -d {{domain_name}} -enum {{index_from_list}} -summary`
