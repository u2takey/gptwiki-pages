# calibredb 
## chatgpt 
calibredb is a command-line tool used to manage eBook libraries in Calibre. It can perform various tasks such as adding, deleting, or updating eBooks, searching for specific titles or authors, and backing up the library.

Here are some of the most commonly used subcommands of calibredb:

1. add: used to add new eBooks to the library. You can specify the path to the eBook file or a directory containing multiple eBooks.

2. delete: to delete eBooks from the library. You can specify the ID of the book or search for it using various criteria such as title, author, or format.

3. list: to view a list of eBooks in the library. You can also use various options to filter and sort the list.

4. search: to search for eBooks with specific criteria such as title, author, tags, or formats.

5. export: to export the library data to a file or as a backup.

6. import: to import library data from a file or another Calibre library.

7. set_metadata: to update the metadata of an eBook such as the title, author, cover image, or tags.

Overall, calibredb is a powerful command-line tool for managing eBook libraries, and it is highly recommended for Calibre users who prefer working with command-line interfaces. 

## tldr 
 
> Tool to manipulate the your e-book database.
> Part of the Calibre e-book library.
> More information: <https://manual.calibre-ebook.com/generated/en/calibredb.html>.

- List e-books in the library with additional information:

`calibredb list`

- Search for e-books displaying additional information:

`calibredb list --search {{search_term}}`

- Search for just ids of e-books:

`calibredb search {{search_term}}`

- Add one or more e-books to the library:

`calibredb add {{file1 file2 …}}`

- Recursively add all e-books under a directory to the library:

`calibredb add -r {{path/to/directory}}`

- Remove one or more e-books from the library. You need the e-book IDs (see above):

`calibredb remove {{id1 id2 …}}`
