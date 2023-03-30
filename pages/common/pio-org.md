# pio org 
## chatgpt 
The command "pio org" is related to the PlatformIO tool for embedded systems development. This command is used to interact with the PlatformIO organization feature, which is used to manage teams and collaborators in PlatformIO projects.

When the "pio org" command is executed, it provides a list of subcommands that can be used to manage organization settings and resources. Some of the commonly used subcommands are:

1. "add": This subcommand is used to add a new member to an organization.

2. "remove": This subcommand is used to remove a member from an organization.

3. "show": This subcommand is used to display information about the organization and its members.

4. "list": This subcommand is used to display a list of all organizations associated with the current user account.

Some additional parameters can also be used with the "pio org" command to specify the name of the organization or the username of the member being added or removed. For example, "pio org add myorganization myuser" will add the user "myuser" to the organization "myorganization".

Overall, the "pio org" command is a useful tool for managing team-based embedded system development projects in PlatformIO. 

## tldr 
 
> Manage PlatformIO organizations and their owners.
> More information: <https://docs.platformio.org/en/latest/core/userguide/org/>.

- Create a new organization:

`pio org create {{organization_name}}`

- Delete an organization:

`pio org destroy {{organization_name}}`

- Add a user to an organization:

`pio org add {{organization_name}} {{username}}`

- Remove a user from an organization:

`pio org remove {{organization_name}} {{username}}`

- List all organizations the current user is a member of and their owners:

`pio org list`

- Update the name, email or display name of an organization:

`pio org update --orgname {{new_organization_name}} --email {{new_email}} --displayname {{new_display_name}} {{organization_name}}`
