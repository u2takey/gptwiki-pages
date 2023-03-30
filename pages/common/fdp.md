# fdp 
## chatgpt 
The command "fdp" is short for "force-directed placement," which is a graph layout algorithm in the Graphviz software suite. The algorithm uses physical simulation to arrange the nodes of a graph in a visually appealing way. 

When using the "fdp" command, a user would typically provide input in the form of a Graphviz DOT file, which describes the structure of a graph using a text-based syntax. The "fdp" command reads this file and computes a layout for the nodes and edges of the graph. 

The algorithm works by treating each node as a repelling point and each edge as an attractive force between its endpoint nodes. The algorithm then simulates the movement of these nodes and edges as if they were particles in space, subject to these forces. Over time, the particles settle into a stable configuration where the nodes and edges are arranged in a visually pleasing way. 

The "fdp" command accepts various options that can be used to customize the layout, such as controlling the strength of the attractive and repulsive forces or setting the width and height of the output image.

Overall, by using the "fdp" command and the Graphviz suite, users can generate attractive and readable visualizations of complex graphs and networks. 

## tldr 
 
> Render an image of a `force-directed` network graph from a `graphviz` file.
> Layouts: `dot`, `neato`, `twopi`, `circo`, `fdp`, `sfdp`, `osage` & `patchwork`.
> More information: <https://graphviz.org/doc/info/command.html>.

- Render a `png` image with a filename based on the input filename and output format (uppercase -O):

`fdp -T png -O {{path/to/input.gv}}`

- Render a `svg` image with the specified output filename (lowercase -o):

`fdp -T svg -o {{path/to/image.svg}} {{path/to/input.gv}}`

- Render the output in a specific format:

`fdp -T {{ps|pdf|svg|fig|png|gif|jpg|json|dot}} -O {{path/to/input.gv}}`

- Render a `gif` image using `stdin` and `stdout`:

`echo "{{digraph {this -> that} }}" | fdp -T gif > {{path/to/image.gif}}`

- Display help:

`fdp -?`
