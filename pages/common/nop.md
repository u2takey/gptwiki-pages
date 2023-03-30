# nop 
## chatgpt 
The nop command, short for "no operation", is a computer instruction that does nothing. It is used as a placeholder in code to indicate where an instruction would normally go, but where no actual operation is needed. 

In assembly language, the nop command specifies a machine instruction that simply advances the program counter to the next instruction in memory, without performing any actual processing. 

In higher-level programming languages, the equivalent of a nop command is typically an empty statement or block, such as a semicolon or curly braces with nothing inside them. 

The primary use of the nop command is to provide a way to align code, optimize instruction execution, or delay operations for timing purposes without altering the functionality of the code. Some processors or compilers may use the nop command for instructions that would otherwise take an excessive amount of time to execute, such as waiting for a slow operation to complete. 

Overall, the nop command is a simple and straightforward instruction that doesn't do anything, but serves an important purpose in computer programming. 

## tldr 
 
> Check validity and pretty-print graphs in canonical format.
> Graphviz filters: `acyclic`, `bcomps`, `comps`, `edgepaint`, `gvcolor`, `gvpack`, `mingle`, `nop`, `sccmap`, `tred`, & `unflatten`.
> More information: <https://www.graphviz.org/pdf/nop.1.pdf>.

- Pretty-print one or more graphs in canonical format:

`nop {{path/to/input1.gv}} {{path/to/input2.gv ...}} > {{path/to/output.gv}}`

- Check one or more graphs for validity, producing no output graph:

`nop -p {{path/to/input1.gv}} {{path/to/input2.gv ...}}`

- Display help for `nop`:

`nop -?`
