# gvpack 
## chatgpt 
`gvpack` is a command-line tool used for merging multiple Graphviz graphs into a single graph. It takes input graphs in Graphviz and pack them into a single output file. 

The general syntax of the `gvpack` command is:

```
gvpack [options] input_files [-o output_file]
```

where `input_files` are the paths of the Graphviz files to be merged and `-o` is an optional parameter for specifying the name and location of the output file.

Some commonly used options with `gvpack` are:

- `-u`: Removes duplicate nodes and edges while merging graphs.
- `-r`: Packs the graphs into a rectangular grid.
- `-s`: Packs the graphs into a single strip.
- `-g`: Pack the graphs into a single, centered graph.

For example, to merge two Graphviz files `graph1.gv` and `graph2.gv` and save the output to a file named `merged.gv`, we can use the following command:

```
gvpack graph1.gv graph2.gv -o merged.gv
```

This command will merge the two graphs and save the output to a file named `merged.gv`. 

## tldr 
 
> Combine several graph layouts (that already have layout information).
> Graphviz filters: `acyclic`, `bcomps`, `comps`, `edgepaint`, `gvcolor`, `gvpack`, `mingle`, `nop`, `sccmap`, `tred`, & `unflatten`.
> More information: <https://graphviz.org/pdf/gvpack.1.pdf>.

- Combine several graph layouts (that already have layout information):

`gvpack {{path/to/layout1.gv}} {{path/to/layout2.gv ...}} > {{path/to/output.gv}}`

- Combine several graph layouts at the graph level, keeping graphs separate:

`gvpack -g {{path/to/layout1.gv}} {{path/to/layout2.gv ...}} > {{path/to/output.gv}}`

- Combine several graph layouts at the node level, ignoring clusters:

`gvpack -n {{path/to/layout1.gv}} {{path/to/layout2.gv ...}} > {{path/to/output.gv}}`

- Combine several graph layouts without packing:

`gvpack -u {{path/to/layout1.gv}} {{path/to/layout2.gv ...}} > {{path/to/output.gv}}`

- Display help for `gvpack`:

`gvpack -?`
