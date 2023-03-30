# traefik 
## chatgpt 
Traefik is a modern and dynamic reverse proxy and load balancer that is designed for microservices and containerized applications. Traefik is written in Go language and designed to manage the traffic between your services, APIs, and applications. 

The command "traefik" is used to run Traefik with its default configuration. When you start the Traefik command, it will listen to incoming HTTP requests on port 80 by default and will route the traffic to the appropriate backend service. 

Here are some important parameters of the "traefik" command:

- "--configFile" or "-c": You can specify the configuration file for Traefik. By default, Traefik uses "traefik.yml", but you can use a different configuration file by adding this parameter followed by the file path.

- "--api": This option enables the Traefik API, which allows you to monitor and manage the Traefik instance using a REST API.

- "--docker": This option enables Traefik's Docker integration, which means that Traefik will automatically discover and update its configuration with the running Docker containers.

- "--loglevel" or "-l": This option sets the logging level for Traefik, allowing you to specify how verbose you want the logs to be.

- "--help" or "-h": This option displays the help documentation for the Traefik command, listing all available options and parameters.

Overall, the "traefik" command is the starting point for running Traefik, and it allows you to customize Traefik's behavior using various options and parameters. 

## tldr 
 
> An HTTP reverse proxy and load balancer.
> More information: <https://traefik.io>.

- Start server with default config:

`traefik`

- Start server with a custom config file:

`traefik --c {{config_file}}.toml`

- Start server with cluster mode enabled:

`traefik --cluster`

- Start server with web UI enabled:

`traefik --web`
