# phar 
## chatgpt 
A phar (PHP archive) is a file format used to distribute PHP applications and libraries in a single package. It allows packaging entire PHP applications or libraries into a single file, which can then be easily distributed and executed on different platforms without the need for an installation process.

To create a phar file, you need to use the phar command, which is a command-line tool that is included in PHP by default. Here is how the command works:

Syntax:

```
php -d phar.readonly=0 phar command [options] [arguments]
```

Explanation:

- `php`: This is the command to execute the php interpreter.
- `-d phar.readonly=0`: This is an optional flag that enables writing to phar archives. By default, phar archives are read-only for security reasons.
- `phar`: This is the actual command to create or manipulate the phar archive.
- `command`: This is the sub-command that specifies the action to perform on the phar archive.
- `[options]`: These are optional flags that modify the behavior of the sub-command.
- `[arguments]`: These are optional arguments that the sub-command requires.

Some common sub-commands of the `phar` command are:

- `build`: This sub-command creates a new phar archive from a list of files and folders.
- `extract`: This sub-command extracts the contents of a phar archive to a directory.
- `list`: This sub-command lists the contents of a phar archive.
- `verify`: This sub-command verifies the integrity of a phar archive.

Example:

To create a new phar archive called "myapp.phar" with the contents of the "src" directory, use the following command:

```
php -d phar.readonly=0 phar build -f myapp.phar src/
```

This command will create a new phar archive called "myapp.phar" that contains all the files and folders in the "src" directory. The `-f` option sets the filename of the phar archive to "myapp.phar". 

## tldr 
 
> Create, update or extract PHP archives (PHAR).
> More information: <https://manned.org/phar>.

- Add space-separated files or directories to a Phar file:

`phar add -f {{path/to/phar_file}} {{files_or_directories}}`

- Display the contents of a Phar file:

`phar list -f {{path/to/phar_file}}`

- Delete the specified file or directory from a Phar file:

`phar delete -f {{path/to/phar_file}} -e {{file_or_directory}}`

- Display full usage information and available hashing/compression algorithms:

`phar help`

- Compress or uncompress files and directories in a Phar file:

`phar compress -f {{path/to/phar_file}} -c {{algorithm}}`

- Get information about a Phar file:

`phar info -f {{path/to/phar_file}}`

- Sign a Phar file with a specific hash algorithm:

`phar sign -f {{path/to/phar_file}} -h {{algorithm}}`

- Sign a Phar file with an OpenSSL private key:

`phar sign -f {{path/to/phar_file}} -h openssl -y {{path/to/private_key}}`
