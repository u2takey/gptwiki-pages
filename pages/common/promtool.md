# promtool 
## chatgpt 
`promtool` is a command-line tool used to interact with and validate Prometheus metrics and configuration files. It is primarily used for troubleshooting and testing Prometheus metrics.

The tool comes with several sub-commands that serve various purposes. Some of the commonly used sub-commands of `promtool` are:

1. check config: This sub-command is used to validate the Prometheus configurations. It checks the syntax and semantics of the configuration file and reports any errors or warnings.

2. check rules: This sub-command is used to validate the Prometheus recording rules and alerting rules. It checks the syntax and semantics of the rules file and reports any errors or warnings.

3. check metrics: This sub-command is used to validate the Prometheus metrics. It checks the syntax and semantics of the metrics and reports any errors or warnings.

4. tsdb: This sub-command is used to interact with the Prometheus time-series database. It can be used to export the database, dump its contents to disk, and apply consistency checks.

In summary, the `promtool` command-line tool is a powerful tool used to validate and interact with Prometheus metrics and configurations. It plays an important role in identifying issues with Prometheus and ensuring that the collected metrics are accurate and consistent. 

## tldr 
 
> Tooling for the Prometheus monitoring system.
> More information: <https://prometheus.io/docs/prometheus/latest/getting_started/>.

- Check if the config files are valid or not (if present report errors):

`promtool check config {{config_file.yml}}`

- Check if the rule files are valid or not (if present report errors):

`promtool check rules {{rules_file.yml}}`

- Pass Prometheus metrics over `stdin` to check them for consistency and correctness:

`curl --silent {{http://example.com:9090/metrics/}} | promtool check metrics`

- Unit tests for rules config:

`promtool test rules {{test_file.yml}}`
