# path 
## chatgpt 
The "path" command in a command line interface is used to display or modify the current system variable called "PATH". 

In simple terms, the PATH variable contains a list of directory paths separated by semicolons (;) that the operating system searches when executing a command. By default, the PATH variable includes paths to commonly used system directories where executable files are located.

Here are some common uses of the "path" command:

- To display the current contents of the PATH variable: 
  - Open a command prompt
  - Type "path" and press enter
  - The output will display a list of directory paths separated by semicolons

- To modify the PATH variable:
  - Open a command prompt with administrator privileges
  - Type "setx PATH "new_path";%PATH%" and press enter (replace "new_path" with the desired directory path)
  - The system should respond with a confirmation message that the PATH variable has been updated

By modifying the PATH variable, you can add or remove directories to control which programs can be executed from the command prompt without specifying the directory path every time. 

## tldr 
 
> Display or set the search path for executable files.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/path>.

- Display the current path:

`path`

- Set the path to one or more semicolon-separated directories:

`path {{path\to\directory1 path\to\directory2 ...}}`

- Append a new directory to the original path:

`path {{path\to\directory}};%path%`

- Set command prompt to only search the current directory for executables:

`path ;`
