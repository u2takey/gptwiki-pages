# aurvote 
## chatgpt 
As an AI language model, I do not have access to your system or the context in which you are using the command "aurvote". However, I can provide you a general explanation of the AUR (Arch User Repository) and the aurvote command.

The AUR is a community-driven repository for Arch Linux packages that allows users to upload their own packages and share them with others. AUR packages are maintained by users and are not part of the official Arch Linux repositories.

The "aurvote" command is a command-line tool for voting on AUR packages. It allows you to upvote or downvote AUR packages based on your experience with them. Your vote helps other users to decide whether to use, modify or maintain a particular package. The command is used in the Terminal or Command Prompt of your computer.

Here are a few examples of how to use the "aurvote" command:

1. To upvote or downvote a package:

aurvote -u [package-name]

Please replace [package-name] with the name of the package you wish to upvote or downvote.

2. To list packages you voted for:

aurvote -l

This command will list all the packages you voted for along with their vote status.

3. To delete your vote for a package:

aurvote -d [package-name]

Please replace [package-name] with the name of the package for which you want to delete your vote.

Note: It is important to provide a useful and honest vote. Misuse of the AUR system can cause issues for others, and it may result in being banned. 

## tldr 
 
> Vote for packages in the Arch User Repository.
> To be able to vote, the file `~/.config/aurvote` must exist and contain your AUR credentials.
> More information: <https://github.com/archlinuxfr/aurvote>.

- Interactively create the file `~/.config/aurvote` containing your AUR username and password:

`aurvote --configure`

- Vote for one or more AUR packages:

`aurvote {{package1 package2 ...}}`

- Unvote one or more AUR packages:

`aurvote --unvote {{package1 package2 ...}}`

- Check if one or more AUR packages have already been voted:

`aurvote --check {{package1 package2 ...}}`

- Show help for `aurvote`:

`aurvote --help`
