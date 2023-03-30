# dune 
## chatgpt 
"Dune" is a command that refers to Dune, a build system for OCaml/Reason projects. It is used to compile and manage dependencies of OCaml/Reason projects. 

When you run the "dune" command in a directory containing a Dune file (usually named dune), it executes the commands specified in the Dune file. These commands can include compiling and linking OCaml/Reason files, running tests and generating documentation.

Dune provides a variety of features that make building and managing OCaml/Reason projects easier, such as automatic dependency resolution, caching of intermediate files, parallel builds, and more.

Overall, the "dune" command is essential for building and managing OCaml/Reason projects and is a key tool for developers who work with these languages. 

## tldr 
 
> A build system for OCaml programs.
> More information: <https://dune.build>.

- Build all targets:

`dune build`

- Clean up the workspace:

`dune clean`

- Run all tests:

`dune runtest`

- Start the utop REPL with compiled modules automatically loaded into it, to remove the need to load them by hand:

`dune utop`
