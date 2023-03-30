# Show-Markdown 
## chatgpt 
As an AI language model, I do not have access to know the full context of the question. But I can provide you with the details about the 'Show-Markdown' command in general.

'Show-Markdown' is a command used in software programs or applications that allows users to preview the formatted text of a document in Markdown language. Markdown is a lightweight text formatting syntax used to create richly structured documents that can easily be converted to HTML or other formats.

When the 'Show-Markdown' command is initiated, it generates a preview of the Markdown document, often displaying the document in a separate window or pane. The preview displays the formatted document as it would appear in HTML, allowing the user to review and adjust any formatting, style or links in the Markdown document. 

Overall, the 'Show-Markdown' command is a particularly useful tool for web developers or content creators who are working on Markdown-based documents or writing for websites that employ Markdown syntax. 

## tldr 
 
> Shows a Markdown file or string in the console in a friendly way using VT100 escape sequences or in a browser using HTML.
> This command can only be used through PowerShell.
> More information: <https://learn.microsoft.com/powershell/module/microsoft.powershell.utility/show-markdown>.

- Render markdown to console from a file:

`Show-Markdown -Path {{path\to\file}}`

- Render markdown to console from string:

`{{"# Markdown content"}} | Show-Markdown`

- Open Markdown file in a browser:

`Show-Markdown -Path {{path\to\file}} -UseBrowser`
