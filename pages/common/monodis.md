# monodis 
## chatgpt 
The "monodis" command is a tool included in the Mono runtime environment that is used to disassemble Microsoft .NET assemblies. When a .NET assembly is compiled, it is converted from human-readable code to binary code that the computer can understand. Monodis works by reverse-engineering the binary code and displaying the original human-readable code. 

The monodis command is used in the following format: 

    monodis [options] assembly_file
    
where "options" are various flags that can be used to modify the output format or behavior of the command, and "assembly_file" is the path to the .NET assembly that you want to disassemble. 

Some of the commonly used options for the monodis command include: 

- -h, --help: Displays a help message with information about the various options that can be used with the command. 

- -c, --casemap: Changes the case of the output to lowercase or uppercase. 

- -d, --detailed: Provides more detailed information about the disassembled code, including information about local variables and exception handlers. 

- -p, --tokenproc: Displays the tokens used internally by the .NET runtime to identify various elements of the code. 

- -r, --raw: Displays the assembly in a raw format, without any additional formatting or indentation. 

Overall, the monodis command is a useful tool for developers who want to analyze or debug .NET assemblies, as it provides a way to view the original source code of the program. 

## tldr 
 
> The Mono Common Intermediate Language (CIL) disassembler.
> More information: <https://www.mono-project.com/docs/tools+libraries/tools/monodis/>.

- Disassemble an assembly to textual CIL:

`monodis {{path/to/assembly.exe}}`

- Save the output to a file:

`monodis --output={{path/to/output.il}} {{path/to/assembly.exe}}`

- Show information about an assembly:

`monodis --assembly {{path/to/assembly.dll}}`

- List the references of an assembly:

`monodis --assemblyref {{path/to/assembly.exe}}`

- List all the methods in an assembly:

`monodis --method {{path/to/assembly.exe}}`

- Show a list of resources embedded within an assembly:

`monodis --manifest {{path/to/assembly.dll}}`

- Extract all the embedded resources to the current directory:

`monodis --mresources {{path/to/assembly.dll}}`
