# autojump 
## chatgpt 
Autojump is a command-line utility that helps you navigate your file system by tracking the directories you frequently visit and allowing you to jump quickly to them using only a few keystrokes. Essentially, it builds a database of directory shortcuts that you can use to navigate your file system more efficiently.

For example, let's say you frequently work in a directory called /home/user/projects/myproject. Normally, you would have to type out the full path every time you wanted to navigate to that directory. With autojump installed, you can simply type "j myproject" (or another shortcut of your choosing) and autojump will take you directly to that directory.

Autojump works by tracking the directories you visit and assigning a weight to each one based on how frequently you visit it. When you enter a shortcut command, autojump looks up the corresponding directory in its database and navigates you there. It also provides tab-completion for your shortcuts, making it easy to find the one you're looking for.

Overall, autojump is a useful tool for anyone who spends a lot of time working in the command line and wants to navigate their file system more efficiently. It's easy to install and use, and can save you time and keystrokes in the long run. 

## tldr 
 
> Quickly jump among the directories you visit the most.
> Aliases like j or jc are provided for even less typing.
> More information: <https://github.com/wting/autojump>.

- Jump to a directory that contains the given pattern:

`j {{pattern}}`

- Jump to a sub-directory (child) of the current directory that contains the given pattern:

`jc {{pattern}}`

- Open a directory that contains the given pattern in the operating system file manager:

`jo {{pattern}}`

- Remove non-existing directories from the autojump database:

`j --purge`

- Show the entries in the autojump database:

`j -s`
