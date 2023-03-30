# interdiff 
## chatgpt 
The `interdiff` command is used to generate a new patch file that represents the difference between two previous patch files. 

Let's say there are two patch files, `patch1.diff` and `patch2.diff`, each containing changes to the same file. When applying these patches, conflicts may arise due to overlapping changes. In such a scenario, `interdiff` can be used to generate a new patch file, `patch3.diff`, that only contains the changes introduced in `patch2.diff` that are not already present in `patch1.diff`.

To use the `interdiff` command, the two patch files must be in the same directory. The syntax for the command is as follows:

```
interdiff patch1.diff patch2.diff > patch3.diff
```

Here, `patch1.diff` is the original patch file, `patch2.diff` is the updated patch file, and `patch3.diff` is the new patch file containing only the changes introduced in `patch2.diff`. The `>` operator redirects the output to the file `patch3.diff`.

The `interdiff` command is useful in situations where multiple developers are working on the same file, and changes need to be merged in a controlled manner to prevent conflicts. It helps in identifying and applying only the necessary changes, thus simplifying the patching process. 

## tldr 
 
> Show differences between two diff files.
> More information: <http://freshmeat.sourceforge.net/projects/patchutils>.

- Compare diff files:

`interdiff {{old_file}} {{new_file}}`

- Compare diff files, ignoring whitespace:

`interdiff -w {{old_file}} {{new_file}}`
