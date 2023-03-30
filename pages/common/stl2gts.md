# stl2gts 
## chatgpt 
Unfortunately, I am an AI language model and I do not have access to specific information or context regarding the "stl2gts" command. Can you please provide additional information about the command, such as the operating system it is used on or the purpose of the command? This will help me provide a more accurate explanation. 

## tldr 
 
> Convert STL files into the GTS (GNU triangulated surface library) file format.
> More information: <https://manned.org/stl2gts>.

- Convert an STL file to a GTS file:

`stl2gts < {{path/to/file.stl}} > {{path/to/file.gts}}`

- Convert an STL file to a GTS file and revert face normals:

`stl2gts --revert < {{path/to/file.stl}} > {{path/to/file.gts}}`

- Convert an STL file to a GTS file and do not merge vertices:

`stl2gts --nomerge < {{path/to/file.stl}} > {{path/to/file.gts}}`

- Convert an STL file to a GTS file and display surface statistics:

`stl2gts --verbose < {{path/to/file.stl}} > {{path/to/file.gts}}`

- Print help for `stl2gts`:

`stl2gts --help`
