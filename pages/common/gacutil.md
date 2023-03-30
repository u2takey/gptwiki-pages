# gacutil 
## chatgpt 
gacutil is a command-line tool that is used to manipulate the Global Assembly Cache (GAC) on Microsoft Windows. The GAC is a central location to store and manage reusable .NET assemblies that are intended to be shared across multiple applications on a computer.

The following are the main commands associated with gacutil:

1. /i – This command installs an assembly into the GAC.

Syntax: gacutil /i <assemblyname>

Example: gacutil /i MyAssembly.dll

2. /u – This command uninstalls an assembly from the GAC.

Syntax: gacutil /u <assemblyname>

Example: gacutil /u MyAssembly.dll

3. /l – This command lists all the assemblies in the GAC.

Syntax: gacutil /l

4. /lr – This command lists all the assemblies in the GAC and also displays their reference count.

Syntax: gacutil /lr

5. /nologo – This command suppresses the display of the copyright and logo information.

Syntax: gacutil /nologo

6. /pause – This command pauses the output after each screenful of information.

Syntax: gacutil /pause

7. /q – This command suppresses all output except error messages.

Syntax: gacutil /q

8. /? – This command displays the command syntax and options.

Syntax: gacutil /? 

## tldr 
 
> Global Assembly Cache (CAG) management utility.
> More information: <https://manned.org/gacutil>.

- Install the specified assembly into GAC:

`gacutil -i {{path/to/assembly.dll}}`

- Uninstall the specified assembly from GAC:

`gacutil -i {{assembly_display_name}}`

- Print the content of GAC:

`gacutil -l`
