# circo 
## chatgpt 
Circo is a command-line program that is used for generating circular layouts of directed graphs. It is part of the Graphviz package of tools that is used for graph visualization, and it has a wide range of options that allow users to customize the layout of the graphs. 

When the "circo" command is executed in the terminal or command prompt, it takes as input a graph description file in a supported format (such as DOT or GXL) and generates an image file (such as PNG or PDF) of the circular layout of the graph. 

Some of the options that can be used with the circo command include:

- -Tformat: this option specifies the output file format (such as PNG, PDF, SVG, etc.)
- -ooutputfile: this option specifies the name of the output file
- -Gsize=size: this option specifies the size of the layout in inches
- -Gresolution=resolution: this option specifies the resolution of the output file
- -Grotate=degrees: this option specifies the rotation angle of the graph
- -Gsplines=true/false: this option determines whether to use splines for the graph edges
- -Nshape=shape: this option specifies the shape of the nodes in the graph
- -Ecolor=color: this option specifies the color of the edges in the graph

Overall, the circo command is a powerful tool for generating circular layouts of directed graphs and allows users to customize the layout and appearance of the graph through various options. 

## tldr 
 
> Render an image of a `circular` network graph from a `graphviz` file.
> Layouts: `dot`, `neato`, `twopi`, `circo`, `fdp`, `sfdp`, `osage` & `patchwork`.
> More information: <https://graphviz.org/doc/info/command.html>.

- Render a `png` image with a filename based on the input filename and output format (uppercase -O):

`circo -T {{png}} -O {{path/to/input.gv}}`

- Render a `svg` image with the specified output filename (lowercase -o):

`circo -T {{svg}} -o {{path/to/image.svg}} {{path/to/input.gv}}`

- Render the output in `ps`, `pdf`, `svg`, `fig`, `png`, `gif`, `jpg`, `json`, or `dot` format:

`circo -T {{format}} -O {{path/to/input.gv}}`

- Render a `gif` image using `stdin` and `stdout`:

`echo "{{digraph {this -> that} }}" | circo -T {{gif}} > {{path/to/image.gif}}`

- Display help:

`circo -?`
