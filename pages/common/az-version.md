# az version 
## chatgpt 
The "az version" command is used in the Azure command-line interface (CLI) to display information about the version of the Azure CLI currently installed on the system.

When this command is executed, it displays the version and build information of the Azure CLI as well as the Python version being used. The output may look similar to the following example:

```
azure-cli                         2.0.75
command-modules-nspkg             2.0.3
core                              2.0.75
telemetry                          1.0.4
Python location '/usr/local/Cellar/python/3.7.3/Frameworks/Python.framework/Versions/3.7/bin/python3'
Extensions:
```

The first line "azure-cli 2.0.75" indicates the version number of the Azure CLI. The second line "command-modules-nspkg 2.0.3" shows the version of the command module packaging while the third line "core 2.0.75" displays the version of the core module. The fourth line "telemetry 1.0.4" indicates the version of the telemetry module. The fifth line "Python location" specifies the location of the Python installation used by Azure CLI. The last line "Extensions:" displays the list of installed Azure CLI extensions.

Overall, the "az version" command is helpful to check the version of Azure CLI and keep track of updates. 

## tldr 
 
> Shows the current version of Azure CLI modules and extensions.
> Part of `az`, the command-line client for Microsoft Azure.
> More information: <https://learn.microsoft.com/cli/azure/reference-index?view=azure-cli-latest#az-version>.

- Show the current version of Azure CLI modules and extensions in JSON format:

`az version`

- Show the current version of Azure CLI modules and extensions in a given format:

`az version --output {{json|table|tsv}}`
