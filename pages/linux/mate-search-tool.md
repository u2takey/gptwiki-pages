# mate-search-tool 
## chatgpt 
The command "mate-search-tool" launches a search tool application called "MATE Search Tool" in the MATE desktop environment. 

MATE Search Tool is a graphical user interface (GUI) search tool that allows users to search for files and folders on their computer by specifying search criteria such as file name, file type, date modified, and more. Once the search criteria are entered, MATE Search Tool quickly displays search results, allowing users to easily find the specific file or folder they are looking for.

In summary, the "mate-search-tool" command launches a file search utility in the MATE desktop environment to help users find specific files and folders on their computer. 

## tldr 
 
> Search files in MATE desktop environment.
> More information: <https://manned.org/mate-search-tool>.

- Search files containing a specific string in their name in a specific directory:

`mate-search-tool --named={{string}} --path={{path/to/directory}}`

- Search files without waiting a user confirmation:

`mate-search-tool --start --named={{string}} --path={{path/to/directory}}`

- Search files with name matching a specific regular expression:

`mate-search-tool --start --regex={{string}} --path={{path/to/directory}}`

- Set a sorting order in search results:

`mate-search-tool --start --named={{string}} --path={{path/to/directory}} --sortby={{name|folder|size|type|date}}`

- Set a descending sorting order:

`mate-search-tool --start --named={{string}} --path={{path/to/directory}} --descending`

- Search files owned by a specific user/group:

`mate-search-tool --start --{{user|group}}={{value}} --path={{path/to/directory}}`
