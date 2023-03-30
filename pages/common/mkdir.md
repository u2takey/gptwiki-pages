# mkdir 
## chatgpt 
The command `mkdir` is a short form of the term "make directory". It is a command that is used in operating systems like Linux, macOS, and Windows to create a new directory or folder.

The syntax for the command is as follows:

```
mkdir [OPTIONS] DIRECTORY
```

- `OPTIONS`: These are optional parameters that can be used to modify the behavior of the command. Some of the common options include `-p`, which creates parent directories if they do not exist, and `-m`, which sets the file mode (permissions) of the directory.
- `DIRECTORY`: This is the name of the directory that you want to create. It can be a relative or absolute path.

Here are some examples of how to use the `mkdir` command:

1. To create a new directory named "documents" in the current directory:

```
mkdir documents
```

2. To create a new directory named "work" inside the "documents" directory:

```
mkdir documents/work
```

3. To create a new directory named "images" and set its file permissions to read-only for others:

```
mkdir -m 444 images
```

4. To create a new directory named "data" and all its parent directories if they do not exist:

```
mkdir -p projects/data
```

Overall, the `mkdir` command is a simple way to create new directories or folders in your file system. It is a useful command for organizing your files and keeping them in separate directories. 

## tldr 
 
> Create directories and set their permissions.
> More information: <https://www.gnu.org/software/coreutils/mkdir>.

- Create specific directories:

`mkdir {{path/to/directory1 path/to/directory2 ...}}`

- Create specific directories and their [p]arents if needed:

`mkdir -p {{path/to/directory1 path/to/directory2 ...}}`

- Create directories with specific permissions:

`mkdir -m {{rwxrw-r--}} {{path/to/directory1 path/to/directory2 ...}}`
