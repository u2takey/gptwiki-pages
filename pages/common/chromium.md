# chromium 
## chatgpt 
The command "chromium" is used to launch the Chromium web browser. Chromium is an open-source web browser that was developed by Google, and it is designed to be fast, secure, and easy to use. 

When you enter the command "chromium" in the terminal or command prompt of your operating system, the browser will be launched and you will be able to start browsing the internet. With Chromium, you can open multiple tabs, browse the web, download files, access your bookmarks and history, and much more.

Chromium is available for various operating systems, including Linux, macOS, and Windows, so the command works on any of these systems. Additionally, since it is an open-source project, you can modify and customize Chromium to suit your needs. 

## tldr 
 
> Open-source web browser principally developed and maintained by Google.
> More information: <https://www.chromium.org/developers/how-tos/run-chromium-with-flags/>.

- Open a specific URL or file:

`chromium {{https://example.com|path/to/file.html}}`

- Open in incognito mode:

`chromium --incognito {{example.com}}`

- Open in a new window:

`chromium --new-window {{example.com}}`

- Open in application mode (without toolbars, URL bar, buttons, etc.):

`chromium --app={{https://example.com}}`

- Use a proxy server:

`chromium --proxy-server="{{socks5://hostname:66}}" {{example.com}}`

- Open with a custom profile directory:

`chromium --user-data-dir={{path/to/directory}}`

- Open without CORS validation (useful to test an API):

`chromium --user-data-dir={{path/to/directory}} --disable-web-security`

- Open with a DevTools window for each tab opened:

`chromium --auto-open-devtools-for-tabs`
