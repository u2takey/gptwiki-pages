# mkfile 
## chatgpt 
The "mkfile" command is used to create a file with a specified size and name on a macOS system. 

The syntax of the command is as follows: 

```
mkfile [size] [filename]
```

The "size" parameter specifies the size of the file to be created, and it is specified in bytes by default. However, you can also use suffixes like "k" for kilobytes, "m" for megabytes, "g" for gigabytes, etc. For example, you can create a 10 MB file by using the command: 

```
mkfile 10m testfile.txt
```

The "filename" parameter specifies the name of the file to be created. You can specify the file path as well, or it will create the file in the current directory by default. 

Once the command is executed, it will create the file with the specified size and name. If the file already exists, the command will overwrite the existing file with the specified size. Therefore, be careful when using this command as it can lead to data loss. 

The "mkfile" command is primarily used by developers and system administrators who need to create files quickly for testing or other purposes. 

## tldr 
 
> Create one or more empty files of any size.
> More information: <https://manned.org/mkfile>.

- Create an empty file of 15 kilobytes:

`mkfile -n {{15k}} {{path/to/file}}`

- Create a file of a given size and unit (bytes, KB, MB, GB):

`mkfile -n {{size}}{{b|k|m|g}} {{path/to/file}}`

- Create two files of 4 megabytes each:

`mkfile -n {{4m}} {{first_filename}} {{second_filename}}`
