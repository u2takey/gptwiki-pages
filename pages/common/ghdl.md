# ghdl 
## chatgpt 
ghdl is a command-line tool used for simulating, analyzing, and synthesizing VHDL code. Here is a breakdown of the command:

Syntax: `ghdl [options] [files]`

Options: There are various options available to use with the ghdl command. Some commonly used ones include:

- `-a`: Analyze a VHDL file, compiling it and generating the corresponding object file.
- `-e`: Elaborate the design entity, creating the simulation executable.
- `-r`: Run a simulation executable or a testbench.
- `-v`: Enable verbose mode, providing more detailed output.
- `-f`: Read the command-line options from a file.
- `-s`: Compile and link multiple VHDL files together into a shared object.

Files: The command can be used to analyze, elaborate, and simulate one or more VHDL files. The files can be specified as VHDL source files (`.vhd` or `.vhdl`) or object files (`.o`).

Examples:

1. To analyze a VHDL file named `example.vhd`:

```
ghdl -a example.vhd
```

2. To elaborate the design entity `top_level` and create a simulation executable:

```
ghdl -e top_level
```

3. To run a simulation executable named `sim`:

```
ghdl -r sim
```

4. To analyze and elaborate multiple VHDL files together:

```
ghdl -a file1.vhd file2.vhd
ghdl -e top_level
```

5. To enable verbose mode:

```
ghdl -v example.vhd
```

Overall, the ghdl command provides a complete toolset for working with VHDL designs, allowing users to compile, simulate, and analyze their code with ease. 

## tldr 
 
> Open-source simulator for the VHDL language.
> More information: <http://ghdl.free.fr>.

- Analyze a VHDL source file and produce an object file:

`ghdl -a {{filename.vhdl}}`

- Elaborate a design (where `{{design}}` is the name of a configuration unit, entity unit or architecture unit):

`ghdl -e {{design}}`

- Run an elaborated design:

`ghdl -r {{design}}`

- Run an elaborated design and dump output to a waveform file:

`ghdl -r {{design}} --wave={{output.ghw}}`

- Check the syntax of a VHDL source file:

`ghdl -s {{filename.vhdl}}`

- Display the help page:

`ghdl --help`
