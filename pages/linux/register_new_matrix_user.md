# register_new_matrix_user 
## chatgpt 
The command "register_new_matrix_user" is a CLI (command line interface) command used to create a new user account on a Matrix server. The Matrix protocol is a decentralized communication platform designed to provide secure and reliable messaging, file sharing, and voice and video calling services.

The command "register_new_matrix_user" is used to create a new user account on a Matrix server. This command takes several parameters such as the username, password, and email address. Once the command is executed, the Matrix server creates a new user account and assigns a unique user ID, known as a Matrix ID, to the user.

The Matrix ID is a unique identifier that is used to represent the user on the Matrix network. It is similar to an email address or a phone number and is used to communicate with other users on the Matrix network.

The "register_new_matrix_user" command is used by server administrators or users with administrative privileges to create new user accounts on the server. It is an important command as it allows new users to join the Matrix network and communicate with other users.

In summary, the "register_new_matrix_user" command is a command-line interface command used to register a new user account on a Matrix server, and it takes several parameters including the username, password, and email address. The command helps to create a unique user ID, which represents the user on the Matrix network. 

## tldr 
 
> Used to register new users with a given home server when registration has been disabled.
> More information: <https://manned.org/register_new_matrix_user>.

- Create a user interactively:

`register_new_matrix_user --config {{path/to/homeserver.yaml}}`

- Create an admin user interactively:

`register_new_matrix_user --config {{path/to/homeserver.yaml}} --admin`

- Create an admin user non-interactively (not recommended):

`register_new_matrix_user --config {{path/to/homeserver.yaml}} --user {{username}} --password {{password}} --admin`
