# acyclic 
## chatgpt 
The `acyclic` command is used to detect cycles in a directed graph or digraph. It takes a graph file as input and returns either a confirmation that the graph is acyclic or a list of cycles present in the graph.

The syntax for using the `acyclic` command is:

```
acyclic [-q] [-v] [-p path] [-f format] [file]
```

Here, `file` is the path to the input graph file, and it can be in any format supported by Graphviz, such as DOT, JSON, or GXL. If no filename is specified, the command reads from the standard input.

The `-q` option suppresses any output, and `-v` produces verbose output during the cycle detection process. The `-p` option specifies a directory path to search for any dependent files, and `-f` specifies the input file format explicitly.

When `acyclic` detects a cycle, it prints out a list of nodes involved in the cycle, separated by arrows. For example, if it detects a cycle involving nodes A, B, and C, it would output:

```
A -> B -> C -> A
```

If the graph is acyclic, `acyclic` simply outputs "graph is acyclic" and exits with status code 0. If any cycles are found, it exits with a non-zero status code. 

## tldr 
 
> Make a directed graph acyclic by reversing some edges.
> Graphviz filters: `acyclic`, `bcomps`, `comps`, `edgepaint`, `gvcolor`, `gvpack`, `mingle`, `nop`, `sccmap`, `tred`, & `unflatten`.
> More information: <https://graphviz.org/pdf/acyclic.1.pdf>.

- Make a directed graph acyclic by reversing some edges:

`acyclic {{path/to/input.gv}} > {{path/to/output.gv}}`

- Print if a graph is acyclic, has a cycle, or is undirected, producing no output graph:

`acyclic -v -n {{path/to/input.gv}}`

- Display help for `acyclic`:

`acyclic -?`
