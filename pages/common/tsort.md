# tsort 
## chatgpt 
tsort is a command line tool in UNIX and Linux operating systems. It is used to perform topological sorting on a directed acyclic graph (DAG). Topological sorting is a linear ordering of the vertices of a graph, where each node comes before all the nodes it points to. 

The command syntax for tsort is:

tsort [file]

The [file] parameter is the name of the file containing the graph. The graph should be in a specific format called the adjacency list format. In this format, each line of the file contains two nodes separated by a space, where the first node is the parent and the second node is the child.

Here is an example file containing a graph:

A B
B C
C D
D E

In this graph, node A has an edge to node B, node B has an edge to node C, node C has an edge to node D, and node D has an edge to node E.

To perform topological sorting on this graph, we can run the tsort command:

tsort graph.txt

The result of this command will be the linear ordering of the vertices in the graph:

A
B
C
D
E

This means that vertex A comes before vertex B, vertex B comes before vertex C, and so on.

If the graph contains cycles, tsort will fail because topological sorting cannot be performed on a graph with cycles. Instead, it will report an error message. 

## tldr 
 
> Perform a topological sort.
> A common use is to show the dependency order of nodes in a directed acyclic graph.
> More information: <https://www.gnu.org/software/coreutils/tsort>.

- Perform a topological sort consistent with a partial sort per line of input separated by blanks:

`tsort {{path/to/file}}`
