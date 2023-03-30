# sfdp 
## chatgpt 
sfdp is a command-line tool that is a part of the Graphviz graph visualization software. 

It stands for "Sparse Matrix-based Graph Layout Program" and is used to generate layouts for large graphs. 

The sfdp command uses a multilevel approach to optimize the layout of the graph. It starts by splitting the graph into smaller subgraphs, and then recursively applies a layout algorithm to each subgraph. 

The resulting layout is optimized for reducing edge crossings and maximizing symmetry, making it easier to analyze and interpret the graph. 

Some of the options available with the sfdp command include controlling the number of levels and the desired aspect ratio of the output graph. 

Overall, the sfdp command can be a useful tool for visualizing large and complex graphs, especially when used in conjunction with other Graphviz tools. 

## tldr 
 
> Render an image of a `scaled force-directed` network graph from a `graphviz` file.
> Layouts: `dot`, `neato`, `twopi`, `circo`, `fdp`, `sfdp`, `osage` & `patchwork`.
> More information: <https://graphviz.org/doc/info/command.html>.

- Render a `png` image with a filename based on the input filename and output format (uppercase -O):

`sfdp -T {{png}} -O {{path/to/input.gv}}`

- Render a `svg` image with the specified output filename (lowercase -o):

`sfdp -T {{svg}} -o {{path/to/image.svg}} {{path/to/input.gv}}`

- Render the output in `ps`, `pdf`, `svg`, `fig`, `png`, `gif`, `jpg`, `json`, or `dot` format:

`sfdp -T {{format}} -O {{path/to/input.gv}}`

- Render a `gif` image using `stdin` and `stdout`:

`echo "{{digraph {this -> that} }}" | sfdp -T {{gif}} > {{path/to/image.gif}}`

- Display help:

`sfdp -?`
