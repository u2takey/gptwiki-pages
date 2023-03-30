# unflatten 
## chatgpt 
The unflatten command is used in the Linux operating system to convert flattened JSON or XML files into a hierarchical format. This command is mainly used to reverse the effect of flattening a JSON or XML file, which means it will help to restore the original structural hierarchy of the file.

The unflatten command takes a flattened JSON or XML file as input and creates a new output file with a hierarchical format based on the original structure of the file. This command is very helpful in data processing and analysis because it helps in easier navigation and understanding of complex data structures.

The syntax of the unflatten command is quite simple, and it only requires the name of the input file and the name of the output file to operate. For example, the command "unflatten input.json > output.json" will take the flattened JSON file named "input.json" and create a new hierarchical JSON file named "output.json".

Overall, the unflatten command is a useful tool for working with JSON or XML files in Linux and helps to simplify and streamline data processing and analysis. 

## tldr 
 
> Adjust directed graphs to improve the layout aspect ratio.
> Graphviz filters: `acyclic`, `bcomps`, `comps`, `edgepaint`, `gvcolor`, `gvpack`, `mingle`, `nop`, `sccmap`, `tred`, & `unflatten`.
> More information: <https://www.graphviz.org/pdf/unflatten.1.pdf>.

- Adjust one or more directed graphs to improve the layout aspect ratio:

`unflatten {{path/to/input1.gv}} {{path/to/input2.gv ...}} > {{path/to/output.gv}}`

- Use `unflatten` as a preprocessor for `dot` layout to improve aspect ratio:

`unflatten {{path/to/input.gv}} | dot -T {{png}} {{path/to/output.png}}`

- Display help for `unflatten`:

`unflatten -?`
