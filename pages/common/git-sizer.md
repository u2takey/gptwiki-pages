# git sizer 
## chatgpt 
`git sizer` is a tool used to analyze the size of files and directories in a git repository. It calculates the disk usage of each file, as well as the percentage of disk usage that each file and directory contributes to the overall repository size.

To use `git sizer`, first ensure that you have it installed on your system. If you are using a Unix-based operating system, you can install it using the following command:

```
curl -s https://raw.githubusercontent.com/github/git-sizer/master/download.sh | bash
```

Once installed, navigate to the root directory of your git repository and run the command `git sizer`.

The output of the command will display the size and percentage contributions of each file and directory in the repository. It will also display any recommendations or warnings if the repository size exceeds certain thresholds, such as the maximum repository size supported by certain hosting platforms.

This information can be useful in identifying large or unnecessary files and directories that may be taking up excessive disk space in the repository. It can also help optimize the repository size and improve overall efficiency. 

## tldr 
 
> Computes various Git repository size metrics and alerts you to any that might cause problems or inconvenience.
> More information: <https://github.com/github/git-sizer>.

- Report only statistics that have a level of concern greater than 0:

`git sizer`

- Report all statistics:

`git sizer -v`

- See additional options:

`git sizer -h`
