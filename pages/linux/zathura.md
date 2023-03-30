# zathura 
## chatgpt 
Zathura is a document viewer that is primarily used to open and view PDF documents, but it also supports other file formats such as PostScript, DjVu, and XPS. 

To use the zathura command, you need to have it installed on your computer. Once installed, you can open a document in zathura by typing:

zathura /path/to/document

This will open the specified document in zathura. Zathura provides a range of keyboard shortcuts that you can use to navigate the document, search for specific text, and adjust the zoom level. You can learn more about these shortcuts by typing:

man zathura

This will display the zathura manual, which provides comprehensive documentation on how to use the software. 

In addition to its basic functionality as a document viewer, zathura can also be customized using plugins. These plugins can extend the application's capabilities, such as allowing you to annotate PDF documents or highlight specific text. To install a plugin, you need to download the plugin file and move it to the appropriate location on your computer. You can then enable the plugin in zathura by editing the application's configuration file. 

Overall, zathura is a versatile document viewer that is highly customizable and provides a range of useful features. 

## tldr 
 
> A vim-like modal document viewer, with an integrated command line.
> Make sure a backend is installed (poppler, PostScript, or DjVu).
> More information: <https://pwmt.org/projects/zathura/>.

- Open a file:

`zathura {{path/to/file}}`

- Navigate left/up/down/right:

`<H|J|K|L> or arrow keys`

- Rotate:

`r`

- Invert Colors:

`Ctrl + R`

- Search for text by a given string:

`/{{string}}`

- Create/delete bookmarks:

`:{{bmark|bdelete}} {{bookmark_name}}`

- List bookmarks:

`:blist`
