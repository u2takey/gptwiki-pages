# neato 
## chatgpt 
neato is a command line tool (program) that is used to visualize graphs and networks, such as those found in data science or computer science. Specifically, neato is a layout engine for creating graph visualizations. 

When invoked, neato takes a text file as input that contains information about the nodes (vertices) and edges in the graph, and then outputs an image file that shows the graph layout. The input file can be in various formats such as .dot, .json, and .svg, among others. 

Neato uses a spring-embedder layout algorithm, which simulates a physical system where nodes are connected by springs and repel each other to minimize overlap. The algorithm is designed to create visually pleasing and readable graphs that clearly show the relationships between nodes. 

Some common options for neato include adjusting the size and shape of the output graph, specifying the output format (e.g. PNG, PDF, SVG), and setting the layout algorithm parameters. 

Overall, neato is a useful tool for visualizing complex networks and making insights into the data. It can be used in a variety of fields including biology, social networking, and transportation systems. 

## tldr 
 
> Render an image of a `linear undirected` network graph from a `graphviz` file.
> Layouts: `dot`, `neato`, `twopi`, `circo`, `fdp`, `sfdp`, `osage` & `patchwork`.
> More information: <https://graphviz.org/doc/info/command.html>.

- Render a `png` image with a filename based on the input filename and output format (uppercase -O):

`neato -T {{png}} -O {{path/to/input.gv}}`

- Render a `svg` image with the specified output filename (lowercase -o):

`neato -T {{svg}} -o {{path/to/image.svg}} {{path/to/input.gv}}`

- Render the output in `ps`, `pdf`, `svg`, `fig`, `png`, `gif`, `jpg`, `json`, or `dot` format:

`neato -T {{format}} -O {{path/to/input.gv}}`

- Render a `gif` image using `stdin` and `stdout`:

`echo "{{graph {this -- that} }}" | neato -T {{gif}} > {{path/to/image.gif}}`

- Display help:

`neato -?`
