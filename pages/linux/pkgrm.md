# pkgrm 
## chatgpt 
The "pkgrm" command is a UNIX command that is used to remove installed software packages. Here's a breakdown of the command:

- "pkgrm" stands for "package remove." It is used to remove a package that has been installed on the system.

- To use the "pkgrm" command, you need to specify the name of the package you want to remove. For example, if you want to remove the "example-package" package, you would run the command "pkgrm example-package" (without the quotation marks).

- When you run the "pkgrm" command, it will remove the files associated with the package, as well as any dependencies that were installed along with it. Dependencies are other packages that are required for the main package to function properly.

- If you try to remove a package that is currently in use or has files that are currently being used by the system, the "pkgrm" command will not allow you to remove it. You will need to shut down any programs that are currently using the package before you can remove it.

- It's important to note that the "pkgrm" command can be a powerful tool, and should be used with care. You should always check the documentation for the package you are removing to make sure that you are using the correct command and that you understand the potential consequences of removing the package. You should also make sure that you have a backup of any important data before you proceed with the removal. 

## tldr 
 
> Remove a package from a CRUX system.
> More information: <https://docs.oracle.com/cd/E86824_01/html/E54764/pkgrm-1m.html>.

- Remove an installed package:

`pkgrm {{package_name}}`
