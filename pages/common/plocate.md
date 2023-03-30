# plocate 
## chatgpt 
The “plocate” command is essentially a tool for finding files and directories on a Linux system. 

To use this command, you will first need to install it on your system. This can usually be done using the package manager for your particular Linux distribution:

- For Debian and Ubuntu, you can install it by running the following command: `sudo apt-get install plocate`
- For CentOS and Fedora, you can install it by running `sudo yum install plocate`

Once you have “plocate” installed, you can use it by simply typing "plocate" followed by the name of the file or directory you are looking for. For example, the command `plocate myfile.txt` would search for any files on the system with the name "myfile.txt".

One reason you might use “plocate” instead of other file search tools is that it uses an indexed database to store and quickly retrieve results. This means that searches are generally faster than with other search tools. The downside is that the initial indexing process can take some time, and the index must be updated periodically in order to stay current.

Some common options for the “plocate” command include:

- `-c`: This option will clear the plocate database and force it to start over with a fresh indexing process.
- `-e`: This option will exclude certain directories or paths from the search process.
- `-i`: This option will perform a case-insensitive search (the default is case-sensitive).
- `-l`: This option will print out the location of the file or directory, as well as some additional information such as permissions and file size.
- `-r`: This option will perform a regular expression search, allowing for more complex search patterns. 

## tldr 
 
> Find filenames quickly.
> Make sure to run `sudo updatedb` to include new files.
> More information: <https://plocate.sesse.net>.

- Look for patterns in the database (recomputed periodically):

`plocate {{pattern}}`

- Look for a file by its exact filename (a pattern containing no globbing characters is interpreted as `*pattern*`):

`plocate */{{filename}}`
