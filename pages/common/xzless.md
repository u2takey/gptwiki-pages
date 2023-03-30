# xzless 
## chatgpt 
The "xzless" command is used to view the contents of a compressed file in a Unix or Linux terminal without extracting it. This command is used in conjunction with the "xz" compression utility, which compresses files into the .xz format.

The "xzless" command works similarly to the "less" command, allowing you to view the contents of a file one page at a time. However, it can only be used on files that have been compressed using the "xz" utility.

To use the "xzless" command, simply type "xzless" followed by the name of the compressed file you wish to view. For example:

```
xzless example_file.xz
```

This will open up the compressed file in a readable format, allowing you to scroll through its contents one page at a time using the arrow keys.

If you want to view a specific part of the file without scrolling, you can add a line number after the file name:

```
xzless example_file.xz 100
```

This will take you directly to line 100 of the file.

Overall, the "xzless" command is a useful tool for quickly viewing the contents of compressed files without having to extract them first. 

## tldr 
 
> Display text from `.xz` and `.lzma` files.
> See also: `less`.
> More information: <https://manned.org/xzless>.

- Open a compressed file:

`xzless {{path/to/archive.xz}}`
