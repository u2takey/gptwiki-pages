# lynx 
## chatgpt 
Lynx is a command-line web browser that allows you to browse the web and view web pages in a text-based format. Here is a detailed explanation of the various aspects of the Lynx command:

Syntax: 

The basic syntax for using the Lynx command is:

lynx [options] [file or URL]

Options:

Lynx has a number of different options that allow you to customize your browsing experience. Some of the most commonly used options include:

- -accept_all_cookies: This option tells Lynx to accept all cookies without prompting the user.
- -force_html: This option tells Lynx to display web pages as HTML even if they are not labeled as HTML.
- -dump: This option tells Lynx to dump the page contents to standard output instead of displaying them in the browser window.
- -verbose: This option tells Lynx to display detailed information about the connection and data transfer process.
- -help: This option displays the Lynx help screen.

File or URL:

Finally, you will need to specify a file or URL to browse using Lynx. This can be either a local file on your system or a website on the internet.

Overall, the Lynx command provides a powerful and flexible way to browse the web without using a graphical web browser. While it may take some time to get accustomed to the text-based interface, Lynx can be a great tool for those who prefer a more minimalistic approach to web browsing. 

## tldr 
 
> Command-line web browser.
> More information: <https://lynx.browser.org>.

- Visit a website:

`lynx {{example.com}}`

- Apply restrictions for anonymous account:

`lynx -anonymous {{example.com}}`

- Turn on mouse support, if available:

`lynx -use_mouse {{example.com}}`

- Force color mode on, if available:

`lynx -color {{example.com}}`

- Open a link, using a specific file to read and write cookies:

`lynx -cookie_file={{path/to/file}} {{example.com}}`

- Navigate forwards and backwards through the links on a page:

`Up arrow key, Down arrow key`

- Go back to the previously displayed page:

`Left arrow key or u`

- Exit:

`q then y`
