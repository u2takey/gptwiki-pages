# envoy 
## chatgpt 
Envoy is an open source, high-performance service proxy that is designed to handle communication among microservices. It is often used as a sidecar proxy within a service mesh architecture.

The envoy command is the primary way to interact with Envoy. When the command is run, it starts up the Envoy process and provides various configuration options to customize its behavior. The command can be used to specify which ports Envoy should listen on, which backends it should route traffic to, and how it should handle different types of traffic.

The envoy command typically requires a configuration file in order to run. This file is written in YAML format and specifies the various configuration options for Envoy. The configuration file can be specified on the command line using the -c or --config-path option, or by setting the ENVOY_PROXY_CONFIG environment variable to the path of the configuration file.

Some common options that can be specified on the envoy command include:

- --config-path/-c: The path to the YAML configuration file
- --admin-address/-a: The address and port where Envoy's admin interface should listen
- --disable-hot-restart/-d: Disables the hot restart feature, which allows Envoy to reload its configuration without downtime
- --log-level/-l: The logging level to use (e.g. trace, debug, info, warning, error, critical)
- --service-cluster/-c: The name of the cluster or service that Envoy is running as part of

Overall, the envoy command is a powerful tool for configuring and running Envoy, which provides a critical piece of infrastructure for building scalable and reliable microservices architectures. 

## tldr 
 
> A PHP-based task manager for Laravel remote servers.
> More information: <https://laravel.com/docs/envoy>.

- Initialize a configuration file:

`envoy init {{host_name}}`

- Run a task:

`envoy run {{task_name}}`

- Run a task from a specific project:

`envoy run --path {{path/to/directory}} {{task_name}}`

- Run a task and continue on failure:

`envoy run --continue {{task_name}}`

- Dump a task as a Bash script for inspection:

`envoy run --pretend {{task_name}}`

- Connect to the specified server via SSH:

`envoy ssh {{server_name}}`
