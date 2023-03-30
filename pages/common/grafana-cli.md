# grafana-cli 
## chatgpt 
Grafana-cli is a command-line interface tool used to manage and maintain Grafana, which is an open-source dashboard and visualization tool. The command "grafana-cli" is used to execute various administration tasks related to Grafana.

The "grafana-cli" command has several subcommands that perform different functions, such as installation, configuration, and plugin management. Some examples of commonly used subcommands include:

- `grafana-cli plugins` - This subcommand is used to manage plugins for Grafana. You can use it to install, update, or remove plugins.

- `grafana-cli admin reset-admin-password` - This subcommand is used to reset the admin password for Grafana.

- `grafana-cli admin enable-auth` - This subcommand is used to enable authentication for Grafana.

- `grafana-cli admin disable-auth` - This subcommand is used to disable authentication for Grafana.

- `grafana-cli admin create-user` - This subcommand is used to create a new user in Grafana.

In summary, "grafana-cli" is an important command-line tool used to manage and maintain Grafana, and has several subcommands that can help you perform various tasks related to Grafana administration. 

## tldr 
 
> A small executable that is bundled with Grafana serve.
> More information: <https://grafana.com/docs/grafana/latest/cli/>.

- Install, update, or remove specific plugins:

`grafana-cli plugins {{install|update|remove}} {{plugin_id1 plugin_id2 ...}}`

- List all installed plugins:

`grafana-cli plugins ls`
