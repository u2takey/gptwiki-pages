# kcadm.sh 
## chatgpt 
The kcadm.sh command is a tool used to interact with Keycloak's Administration REST API. Keycloak is an authentication and authorization solution developed by Red Hat, which provides an identity management system that allows users to authenticate with their own identities or 3rd party providers. The kcadm.sh tool can be used to manage Keycloak's resources such as realms, users, roles, clients, etc.

The 'kcadm.sh' command is typically run from the command line on a Keycloak server and provides a set of sub-commands to interact with Keycloak. The tool is written in shell script and uses the curl command to interact with the API.

The syntax for using the kcadm.sh command is as follows:

```
kcadm.sh [options] <command> [command options]
```

For example, to create a new realm in Keycloak using kcadm.sh, we can use the following command:

```
kcadm.sh create realms -s realm=myrealm -s enabled=true
```

In this example, we are using the 'create' sub-command to create a new realm in Keycloak. We pass in the 'realms' resource type and set two parameters: 'realm' to specify the name of the new realm, and 'enabled' to specify whether the new realm should be enabled or not.

Overall, the kcadm.sh command is a powerful tool for managing Keycloak resources through the Administration REST API. It allows users to automate and streamline the management of Keycloak, making it easier to manage large numbers of users, roles, clients, and other resources. 

## tldr 
 
> Perform administration tasks from the command-line interface (CLI).
> More information: <https://www.keycloak.org/docs/latest/server_admin/#admin-cli>.

- Start an authenticated session:

`kcadm.sh config credentials --server {{host}} --realm {{realm_name}} --user {{username}} --password {{password}}`

- Create a user:

`kcadm.sh create users -s username={{username}} -r {{realm_name}}`

- List all realms:

`kcadm.sh get realms`

- Update a realm with JSON config:

`kcadm.sh update realms/{{realm_name}} -f {{path/to/file.json}}`
