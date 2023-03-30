# autoconf 
## chatgpt 
Autoconf is a tool used to create configure scripts for building, configuring and installing software on Unix and Unix-like systems. A configuration script is a shell script that checks the user's system for various programs, libraries, and features required by the software being built or installed. 

When the autoconf command is run, it reads a file named "configure.ac" or "configure.in" in the current directory and generates a "configure" script. The "configure" script is then used to check the capabilities of the user's system and generate a "Makefile" for building and installing the software. 

The "configure.ac" or "configure.in" file contains macros written in the M4 macro language that define the features required by the software being built. These macros are expanded by the autoconf command to generate the "configure" script. 

Autoconf also supports a number of options that can be passed on the command line. For example, the "--prefix" option can be used to specify where the software should be installed. The "--help" option displays a list of available options. 

## tldr 
 
> Generate configuration scripts to automatically configure software source code packages.
> More information: <https://www.gnu.org/software/autoconf>.

- Generate a configuration script from `configure.ac` (if present) or `configure.in` and save this script to `configure`:

`autoconf`

- Generate a configuration script from the specified template; output to `stdout`:

`autoconf {{template-file}}`

- Generate a configuration script from the specified template (even if the input file has not changed) and write the output to a file:

`autoconf --force --output={{outfile}} {{template-file}}`
