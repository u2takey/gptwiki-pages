# tlmgr option 
## chatgpt 
The command "tlmgr option" is a command in TeX Live Manager that allows you to view and modify the options for the TeX Live distribution.

When you run the command "tlmgr option", you will see a list of available options. These options are divided into categories such as network, repository, and paper size. Some examples of the options you might see include:

- "preferred-repositories": This option allows you to specify which TeX Live repositories to use for package installation and updates.
- "synctex": This option enables or disables Synctex, a synchronization tool that allows you to jump between the source code and the compiled output in a PDF viewer.
- "papersize": This option sets the default paper size for all documents you create with TeX Live.

To modify an option, you can run the command "tlmgr option <option_name> <value>". For example, to set the default paper size to A4, you would run "tlmgr option papersize a4".

It's worth noting that some options can only be modified by the system administrator, or may require additional configuration changes in order to take effect. Be sure to consult the TeX Live Manager documentation for more information on each option. 

## tldr 
 
> TeX Live settings manager.
> More information: <https://www.tug.org/texlive/tlmgr.html>.

- List all TeX Live settings:

`tlmgr option showall`

- List all currently set Tex Live settings:

`tlmgr option show`

- Print all TeX Live settings in JSON format:

`tlmgr option showall --json`

- Show the value of a specific TeX Live setting:

`tlmgr option {{setting}}`

- Modify the value of a specific TeX Live setting:

`tlmgr option {{setting}} {{value}}`

- Set TeX Live to get future updates from the internet after installing from DVD:

`tlmgr option {{repository}} {{https://mirror.ctan.org/systems/texlive/tlnet}}`
