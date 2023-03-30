# texdoc 
## chatgpt 
The command "texdoc" is used to access the documentation files for TeX, LaTeX, and related packages installed on a system. Here are some details about the command:

1. The command "texdoc" can be used in the terminal/command prompt/console of a computer. It is available on most Tex distributions including TeX Live, MiKTeX, and MacTeX.

2. When "texdoc" is followed by a package or document name, it will open the corresponding documentation file in a PDF viewer that is installed on the system. For example, running "texdoc amsmath" will open the documentation of the amsmath package.

3. In addition to PDFs, "texdoc" can also open HTML or plain text documentation files. If a PDF file is not available for a given package or document, it will return a list of alternative formats available.

4. Apart from opening documentation files, "texdoc" can also be used to search for packages or documents that match a particular keyword. The command "texdoc -l keyword" will list all available packages with matching keywords.

5. The "texdoc" command can be used with options to customize its behavior. Some examples of options include "-m" for displaying the package's maintainer and "-s" for searching for documentation files stored in a specific directory.

Overall, "texdoc" is a very helpful command for accessing and navigating the vast documentation library available for TeX and LaTeX. 

## tldr 
 
> Search for appropriate documentation for (La)TeX commands or packages.
> More information: <https://texdoc.org/index.html>.

- Open the first search result in the default PDF viewer:

`texdoc {{search}}`

- List the best search results:

`texdoc --list {{search}}`

- Open full documentation of texdoc:

`texdoc {{texdoc}}`
