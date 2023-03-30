# colorls 
## chatgpt 
`colorls` is a command-line utility that is similar to the traditional `ls` command. However, it adds some aesthetic and functional features to the output of `ls` making it easier to read and visually appealing. 

The `colorls` command works by colorizing the output of `ls`, making it easier to distinguish between different file types, directories, or links. Different types of files and directories are assigned unique colors, and this helps in easily identifying them, even when listed together. For instance, directories are usually shown in blue, executables appear in green, and symbolic links in magenta. 

`colorls` also provides additional formatting options such as displaying file sizes and permissions in a more readable format. It can also display icons for different file types to make it more visually appealing.

One of the key benefits of `colorls` is that it can save the output in various formats, including HTML and Markdown, giving users the option of sharing and presenting file listings in different formats and styles.

In summary, `colorls` is an intuitive and visually appealing command-line utility that enhances the user experience of listing and browsing files on a Unix-based operating system. 

## tldr 
 
> A Ruby gem that beautifies the terminal's ls command, with color and font-awesome icons.
> More information: <https://github.com/athityakumar/colorls>.

- List files one per line:

`colorls -1`

- List all files, including hidden files:

`colorls --all`

- Long format list (permissions, ownership, size, and modification date) of all files:

`colorls --long --all`

- Only list directories:

`colorls --dirs`
