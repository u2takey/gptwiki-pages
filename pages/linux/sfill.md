# sfill 
## chatgpt 
The `sfill` command is a secure version of the `fill` command, which is used to write data onto a specific file or device. The primary purpose of the `sfill` command is to securely overwrite the contents of a file with random data to prevent it from being recovered. 

The `sfill` command can be used with various options and parameters, which are explained below:

Syntax: `sfill [OPTIONS] [FILES OR DIRECTORIES]`

Options:

1. `-f` or `--force`: This option is used to force overwriting of files without any prompts or confirmation.

2. `-v` or `--verbose`: This option is used to print the progress of the command on the terminal.

3. `-l` or `--random`: This option is used to fill the file with random data to make sure that the contents of the file are completely overwritten.

4. `-z` or `--zero`: This option is used to fill the file with zeroes (0) instead of random data.

5. `-n` or `--iterations`: This option is used to specify the number of times that the file should be overwritten with random data or zeroes. By default, the file is overwritten only once.

6. `-p` or `--sprogress`: This option is used to show the progress of overwriting the file.

7. `-r` or `--remove`: This option is used to remove the file securely by overwriting its contents with random data or zeroes before deleting it.

8. `-x` or `--extended` : This option is used to overwrite not only the file contents, but also the metadata associated with the file, such as file name and size.

Examples:

1. `sfill -f myfile.txt` : This command overwrites the contents of the file "myfile.txt" with random data without any prompts or confirmation.

2. `sfill -z -l -n 3 mydir` : This command fills all the files inside the directory "mydir" with zeroes and overwrites them three times to ensure that previous data cannot be recovered.

3. `sfill -r sensitivefile.txt` : This command overwrites the contents of the file "sensitivefile.txt" with random data and then deletes the file securely.

Overall, the `sfill` command is a useful tool for ensuring that sensitive information cannot be recovered from a file or device, and it is recommended to use it regularly to protect your data. 

## tldr 
 
> Securely overwrite the free space and inodes of the partition where the specified directory resides.
> More information: <https://manned.org/sfill>.

- Overwrite free space and inodes of a disk with 38 writes (slow but secure):

`sfill {{/path/to/mounted_disk_directory}}`

- Overwrite free space and inodes of a disk with 6 writes (fast but less secure) and show status:

`sfill -l -v {{/path/to/mounted_disk_directory}}`

- Overwrite free space and inodes of a disk with 1 write (very fast but insecure) and show status:

`sfill -ll -v {{/path/to/mounted_disk_directory}}`

- Overwrite only free space of a disk:

`sfill -I {{/path/to/mounted_disk_directory}}`

- Overwrite only free inodes of a disk:

`sfill -i {{/path/to/mounted_disk_directory}}`
