# buku 
## chatgpt 
The "buku" command is a Linux command line tool for managing and organizing bookmarks. It is used to store and retrieve bookmarks of web pages or files in one place so that users can easily access them later.

When the "buku" command is executed on the Linux terminal, it will open the "buku" command line interface, which provides various options to manage bookmarks, including:

1. Adding bookmarks: Users can add bookmarks to "buku" by typing "buku add" followed by the URL or file path they want to bookmark. They can also add tags and notes to the bookmark for better organization and searchability.

2. Searching bookmarks: Users can search for bookmarks using keywords, tags, or note contents through the "buku" search interface.

3. Editing bookmarks: The "buku" command also provides editing options for bookmarks, which include changing the bookmark URL, adding or removing tags, changing notes, etc.

4. Deleting bookmarks: Users can remove bookmarks by using the "buku delete" command followed by the bookmark number or the bookmark URL.

Other useful features of the "buku" command include exporting bookmarks to various formats such as JSON, HTML, and Markdown, as well as importing bookmarks from various sources like web browsers, CSV files, and Pocket. 

In summary, the "buku" command is a powerful and versatile tool for bookmark management on Linux systems. 

## tldr 
 
> Command-line browser-independent bookmark manager.
> More information: <https://github.com/jarun/Buku>.

- Display all bookmarks matching "keyword" and with "privacy" tag:

`buku {{keyword}} --stag {{privacy}}`

- Add bookmark with tags "search engine" and "privacy":

`buku --add {{https://example.com}} {{search engine}}, {{privacy}}`

- Delete a bookmark:

`buku --delete {{bookmark_id}}`

- Open editor to edit a bookmark:

`buku --write {{bookmark_id}}`

- Remove "search engine" tag from a bookmark:

`buku --update {{bookmark_id}} --tag {{-}} {{search engine}}`
