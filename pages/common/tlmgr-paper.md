# tlmgr paper 
## chatgpt 
As an AI language model, I do not have direct access to command line or the context surrounding the command. However, I can explain to you the possible function and syntax of the command "tlmgr paper". 

The command "tlmgr paper" is likely a sub-command of the TeX Live Manager (tlmgr) utility. The tlmgr command is used to manage installations of TeX Live, a popular typesetting system used for creating documents with complex layouts such as scientific papers, presentations, and books.

The "paper" sub-command is most likely used to manage the selection of paper sizes for TeX Live. Specifically, it could be used to install or remove paper size packages or to list available paper sizes.

The syntax of the command would depend on the specific flags and options used with the "paper" sub-command. Without context, it's difficult to provide more specific information about the syntax of this command. 

## tldr 
 
> Manage paper size options of an TeX Live installation.
> More information: <https://www.tug.org/texlive/tlmgr.html>.

- Show the default paper size used by all TeX Live programs:

`tlmgr paper`

- Set the default paper size for all TeX Live programs to A4:

`sudo tlmgr paper {{a4}}`

- Show the default paper size used by a specific TeX Live program:

`tlmgr {{pdftex}} paper`

- Set the default paper size for a specific TeX Live program to A4:

`sudo tlmgr {{pdftex}} paper {{a4}}`

- List all available paper sizes for a specific TeX Live program:

`tlmgr {{pdftex}} paper --list`

- Dump the default paper size used by all TeX Live programs in JSON format:

`tlmgr paper --json`
