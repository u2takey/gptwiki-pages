# libreoffice 
## chatgpt 
LibreOffice is a command that launches the LibreOffice software suite. LibreOffice is a free and open-source office productivity software suite that includes several applications, such as Writer (word processing), Calc (spreadsheet), Impress (presentation), Draw (vector graphics and flowcharts), and Base (database management). 

When the LibreOffice command is executed in a terminal or command prompt, it launches the LibreOffice suite, and the user can select one of the applications to use. Each application has its own set of features and tools, allowing users to create, edit, and manage various types of documents such as text documents, spreadsheets, presentations, diagrams, and databases.

LibreOffice is a cross-platform suite, which means it is available for several operating systems such as Windows, macOS, and Linux. LibreOffice is a popular alternative to proprietary office suites such as Microsoft Office, offering users an open-source solution for their productivity needs. Overall, the LibreOffice command provides access to a powerful suite of office applications that can be used for personal, educational, or professional purposes. 

## tldr 
 
> CLI for the powerful and free office suite LibreOffice.
> More information: <https://www.libreoffice.org/>.

- Open a space-separated list of files in read-only mode:

`libreoffice --view {{path/to/file1}} {{path/to/file2}}`

- Display the content of specific files:

`libreoffice --cat {{path/to/file1}} {{path/to/file2}}`

- Print files to a specific printer:

`libreoffice --pt {{printer_name}} {{path/to/file1}} {{path/to/file2}}`

- Convert all `.doc` files in current directory to PDF:

`libreoffice --convert-to {{pdf}} {{*.doc}}`
