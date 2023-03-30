# duc 
## chatgpt 
As an AI language model, I have come across different meanings for the acronym "DUC." However, based on my research, the most common interpretation of the term is that it is a command-line utility tool that helps in analyzing disk usage in a Unix or Unix-like operating system. 

The command "duc" is used to display disk usage stats in a structured and sorted format. It can be used to locate files and directories that are consuming the most disk space on your system, which can help to optimize storage usage. 

The syntax of the "duc" command may vary based on the specifics of the operating system it is being used on. However, here is an example Unix command that displays the total size of each directory and its subdirectories within the current directory, sorted in decreasing order of size:

`duc sort -s -n -c -f '6 GB' .`

- `sort` - This option sorts the output in decreasing order of size.
- `-s` - This option shows the size of each directory.
- `-n` - This option shows the number of files and directories in each directory.
- `-c` - This option is used to enable color output.
- `-f '6 GB'` - This option filters out directories smaller than 6GB.
- `.` - The dot refers to the current working directory.

When you run the above command, you will be able to view the disk space occupied by different directories in the current directory, and you can take necessary actions to optimize the disk space accordingly. Note that you may need to have administrative privileges to run this command on certain systems. 

## tldr 
 
> Duc is a collection of tools for indexing, inspecting and visualizing disk usage. Duc maintains a database of accumulated sizes of directories of the file system, allowing queries this database, or create fancy graphs to show where data is.
> More information: <https://duc.zevv.nl/>.

- Index the /usr directory, writing to the default database location ~/.duc.db:

`duc index {{/usr}}`

- List all files and directories under /usr/local, showing relative file sizes in a [g]raph:

`duc ls -Fg {{/usr/local}}`

- List all files and directories under /usr/local using treeview recursively:

`duc ls -Fg -R {{/usr/local}}`

- Start the graphical interface to explore the file system using sunburst graphs:

`duc gui {{/usr}}`

- Run the ncurses console interface to explore the file system:

`duc ui {{/usr}}`

- Dump database info:

`duc info`
