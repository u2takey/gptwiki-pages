# diffoscope 
## chatgpt 
The `diffoscope` command is a tool for comparing files and directories in a detailed and intelligent way. It works by analyzing the contents of files and directories and highlighting differences, even when the files are in different file formats or have been processed in different ways.

Here are some of the main features of `diffoscope`:

- File format support: `diffoscope` can compare files in a wide variety of formats, including archives (like tarballs and zip files), binary executables, firmware images, disk images, and more. It has built-in support for many common file types and can also use external tools to handle more specialized formats.

- Deep analysis: `diffoscope` goes beyond just comparing file contents byte-by-byte. It can analyze files at a higher level, looking for things like differences in file headers, metadata, and other information that may be important for certain use cases.

- Detailed output: `diffoscope` produces output that makes it easy to see exactly what is different between two files or directories. It includes side-by-side comparisons, line-by-line differences, and color highlighting to help make the differences easy to read.

- Automatable: `diffoscope` can be used in scripts and automated workflows, making it useful for things like continuous integration testing and checking for subtle differences in large sets of files.

Overall, `diffoscope` is a powerful tool for anyone who needs to compare files or directories in a detailed and intelligent way. Its wide support for file formats and deep analysis capabilities make it useful in a variety of contexts, from software development to digital forensics. 

## tldr 
 
> Compare files, archives, and directories.
> More information: <https://diffoscope.org>.

- Compare two files:

`diffoscope {{path/to/file1}} {{path/to/file2}}`

- Compare two files without displaying a progress bar:

`diffoscope --no-progress {{path/to/file1}} {{path/to/file2}}`

- Compare two files and write an HTML-report to a file (use `-` for `stdout`):

`diffoscope --html {{path/to/outfile|-}} {{path/to/file1}} {{path/to/file2}}`

- Compare two directories excluding files with a name matching a specified pattern:

`diffoscope --exclude {{pattern}} {{path/to/directory1}} {{path/to/directory2}}`

- Compare two directories and control whether directory metadata is considered:

`diffoscope --exclude-directory-metadata {{auto|yes|no|recursive}} {{path/to/directory1}} {{path/to/directory2}}`
