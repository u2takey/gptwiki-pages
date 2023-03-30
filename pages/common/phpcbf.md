# phpcbf 
## chatgpt 
phpcbf is a command-line tool used for automatically correcting coding standards in PHP code according to the PSR standards or any other custom coding standards defined by the user. 

Here is a breakdown of the command:

- `phpcbf`: This is the actual command that executes phpcbf on the command line.
- `-d`: This option is used to define a PHP configuration file that phpcbf should use. This is optional.
- `-n`: This option tells phpcbf to not make changes to the file system when running. It is typically used for testing purposes.
- `--standard`: This option specifies the coding standard to use when fixing code. The PSR standard is the default, but other popular standards like PEAR, Zend or Symfony can also be specified. Users may also specify their own custom coding standards instead.
- `file.php`: This specifies the file or directory to apply phpcbf on. If a directory is specified, phpcbf will apply the changes to all the PHP files in that directory and its subdirectories.

To use phpcbf, simply run the command followed by the options and file/directory path. phpcbf will then analyze the code, identify any coding standard violatiosn and apply the necessary corrections. 

## tldr 
 
> Fix violations detected by phpcs.
> More information: <https://github.com/squizlabs/PHP_CodeSniffer>.

- Fix issues in the specified directory (defaults to the PEAR standard):

`phpcbf {{path/to/directory}}`

- Display a list of installed coding standards:

`phpcbf -i`

- Specify a coding standard to validate against:

`phpcbf {{path/to/directory}} --standard {{standard}}`

- Specify comma-separated file extensions to include when sniffing:

`phpcbf {{path/to/directory}} --extensions {{file_extension(s)}}`

- A comma-separated list of files to load before processing:

`phpcbf {{path/to/directory}} --bootstrap {{file(s)}}`

- Don't recurse into subdirectories:

`phpcbf {{path/to/directory}} -l`
