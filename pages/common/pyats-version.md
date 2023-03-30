# pyats version 
## chatgpt 
The command "pyats version" is used to display the current version of the pyATS package installed in the system.

PyATS is a Python Test Automation Framework developed by Cisco. It provides a set of APIs for automating network testing and validation. PyATS helps in creating automated testing scripts to verify network functionality, performance, security, and other aspects.

When the "pyats version" command is executed, it calls the pyats package installed in the system and displays the version number of the currently installed package. This command is useful in identifying which version of PyATS is installed and to check whether it matches the requirements of the test scripts being developed.

The output of the "pyats version" command would display the version number in the format of X.Y.Z where X is major version, Y is minor version, and Z is the patch version. For example, if the output of the "pyats version" command is "pyATS version 21.7.1", it means that PyATS version 21.7.1 is installed on the system. 

## tldr 
 
> View and upgrade the pyATS installation.
> More information: <https://developer.cisco.com/pyats/>.

- Display version of all packages:

`pyats version check`

- Display outdated packages:

`pyats version check --outdated`

- Update packages to the most recent version:

`pyats version update`

- Update or downgrade packages to a specific version:

`pyats version update {{version}}`
