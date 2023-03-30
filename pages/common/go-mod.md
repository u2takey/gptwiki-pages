# go mod 
## chatgpt 
The command "go mod" is used in Go programming language to manage modules. The modules in Go is a way to organize code and dependencies of a program. It is used to enable reproducible builds and to avoid conflicts between dependencies. The "go mod" command is used to perform various tasks related to the modules. 

Some of the tasks that can be performed using "go mod" command are:

- Initiate a new module: This task can be performed by using "go mod init" command followed by the name of the module. This creates a new file named "go.mod" in the current directory which contains the metadata of the module.
- Add or remove dependencies: Dependencies can be added to a module using "go mod tidy" command which fetches and adds all the dependencies listed in "go.mod" file. Dependencies can also be added manually by using "go get <dependency_name>" command followed by the name of the dependency. Similarly, dependencies can be removed using "go mod tidy" command and by manually removing the dependency from "go.mod" file.
- Update dependencies: Dependencies can be updated to their latest version using "go get -u" command followed by the name of the dependency. The version of the dependency can be pinned by using "go get <dependency_name>@<version>" command. The updated versions can also be added manually to "go.mod" file.
- Vendor dependencies: This task can be performed using "go mod vendor" command which copies all the dependencies listed in "go.mod" file to the "vendor" directory of the module. This is useful for ensuring the availability of dependencies while building the module.
- Verify dependencies: The dependencies in a module can be verified for security and authenticity using "go mod verify" command which checks the checksums of the downloaded dependencies against the checksums listed in "go.sum" file.

In summary, the "go mod" command is a powerful tool to manage modules in Go programming language. It provides various features for initializing, adding, removing, updating, and verifying dependencies of a module. 

## tldr 
 
> Module maintenance.
> More information: <https://golang.org/cmd/go/#hdr-Module_maintenance>.

- Initialize new module in current directory:

`go mod init {{moduleName}}`

- Download modules to local cache:

`go mod download`

- Add missing and remove unused modules:

`go mod tidy`

- Verify dependencies have expected content:

`go mod verify`

- Copy sources of all dependencies into the vendor directory:

`go mod vendor`
