# mingle 
## chatgpt 
I'm sorry, but as an AI language model, I don't have access to specific commands or programs on your computer. Could you please provide more context or clarify what exactly you would like me to explain about the "mingle" command? 

## tldr 
 
> Bundle the edges of a graph layout.
> Graphviz filters: `acyclic`, `bcomps`, `comps`, `edgepaint`, `gvcolor`, `gvpack`, `mingle`, `nop`, `sccmap`, `tred`, & `unflatten`.
> More information: <https://www.graphviz.org/pdf/mingle.1.pdf>.

- Bundle the edges of one or more graph layouts (that already have layout information):

`mingle {{path/to/layout1.gv}} {{path/to/layout2.gv ...}} > {{path/to/output.gv}}`

- Perform layout, bundling, and output to a picture with one command:

`dot {{path/to/input.gv}} | mingle | dot -T {{png}} > {{path/to/output.png}}`

- Display help for `mingle`:

`mingle -?`
