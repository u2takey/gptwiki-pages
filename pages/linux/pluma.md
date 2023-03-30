# pluma 
## chatgpt 
Pluma is a command used in Linux operating systems to open the Pluma text editor. 

The Pluma text editor is a lightweight and easy-to-use software for creating and editing text files in Linux. It is similar to other popular text editors such as Notepad++ (Windows) and Gedit (Linux). The Pluma editor includes features such as syntax highlighting, auto-indentation, and spell-checking.

To use the pluma command, simply open a terminal window and type "pluma" followed by the name/path of the file you wish to open. For example, if you want to open a file called "myfile.txt" located in your home directory, you would enter the following command:

pluma ~/myfile.txt

This will launch the Pluma text editor with "myfile.txt" already loaded and ready for editing. From here you can use the various tools and options available in Pluma to modify and save your text file. Once you have finished editing, you can close the editor and return to the terminal prompt. 

## tldr 
 
> Edit files in MATE desktop environment.
> More information: <https://manned.org/pluma>.

- Start the editor:

`pluma`

- Open specific documents:

`pluma {{path/to/file1 path/to/file2 ...}}`

- Open documents using a specific encoding:

`pluma --encoding {{WINDOWS-1252}} {{path/to/file1 path/to/file2 ...}}`

- Print all supported encodings:

`pluma --list-encodings`

- Open document and go to a specific line:

`pluma +{{10}} {{path/to/file}}`
