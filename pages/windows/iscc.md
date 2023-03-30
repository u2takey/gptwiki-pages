# iscc 
## chatgpt 
iscc is a command-line tool used for creating Inno Setup installers. Inno Setup is a free installer for Windows programs that provides a customizable installation experience with support for multiple languages, shortcuts, registry entries, and more.

The iscc command is used to compile a script file (.iss) into an executable installer (.exe). To use the iscc command, you must have a valid Inno Setup script file that defines the installation process of your program.

The basic syntax of the iscc command is as follows:

iscc [options] script_name.iss

Where [options] are optional command-line arguments that modify the compilation process, and script_name.iss is the name of the Inno Setup script file that you want to compile.

The iscc command supports several options that can be used to customize the installer, including:

- /o - specifies the output directory for the generated installer file.
- /d - specifies a preprocessor's define to be used during compilation.
- /n - specifies the "Name" parameter for the installer.
- /p - specifies the "Publisher" parameter for the installer.
- /q - specifies the "Quiet" parameter for the installer.

Once you run the iscc command with the appropriate options and script file, it will compile the script into a standalone executable installer that can be distributed and run on Windows systems. 

## tldr 
 
> Compiler for Inno Setup installers.
> It compiles an Inno Setup scripts into an Windows installer executable.
> More information: <https://jrsoftware.org/isinfo.php>.

- Compile an Inno Setup script:

`iscc {{path\to\file.iss}}`

- Quietly compile an Inno Setup installer:

`iscc /Q {{path\to\file.iss}}`

- Compile a signed Inno Setup installer:

`iscc /S={{name}}={{command}} {{path\to\file.iss}}`
