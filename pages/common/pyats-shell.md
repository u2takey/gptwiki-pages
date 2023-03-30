# pyats shell 
## chatgpt 
The `pyats shell` command is used to start an interactive Python console with the pyATS framework pre-loaded. 

PyATS is a Python-based framework that enables users to create and run automated tests for network devices. It provides libraries that simplify tasks such as configuring devices, running tests, and reporting results.

When the `pyats shell` command is executed, it first checks if pyATS is already installed. If not, it will install it along with any required dependencies. Once the framework is installed, a Python shell will be launched with the pyATS modules pre-imported for use.

From here, users can write and execute Python code using the pyATS libraries, which includes functions for connecting to network devices, performing network testing, and analyzing results.

Overall, the `pyats shell` command is a convenient way to quickly launch an interactive console that is ready to work with the pyATS framework. 

## tldr 
 
> Start a pre-loaded pyATS interactive Python Shell to save time in prototyping.
> More information: <https://pubhub.devnetcloud.com/media/genie-docs/docs/cli/genie_shell.html>.

- Open pyATS shell with a defined Testbed file:

`pyats shell --testbed-file {{path/to/testbed.yaml}}`

- Open pyATS shell with a defined Pickle file:

`pyats shell --pickle-file {{path/to/pickle.file}}`

- Open pyATS with IPython disabled:

`pyats shell --no-ipython`
