# firefox 
## chatgpt 
Firefox is a web browser developed by Mozilla Foundation. The command "firefox" when executed, launches the Firefox web browser on your computer. It is an executable command that launches the Firefox application, and the user can utilize it to browse the internet, visit websites, and interact with web applications.

When executed, the command may open a new window, or bring a previously opened window to the front, depending on the user's browser configuration. Firefox is a highly configurable browser that provides multiple features, including a tabbed interface, support for extensions and add-ons, and private modes of browsing to ensure user privacy.

In summary, the "firefox" command is used to launch the Firefox web browser and allow users to surf the internet, interact with websites, and use various browser features available in the Firefox browser. 

## tldr 
 
> A free and open source web browser.
> More information: <https://developer.mozilla.org/en-US/docs/Mozilla/Command_Line_Options>.

- Launch Firefox and open a web page:

`firefox {{https://www.duckduckgo.com}}`

- Open a new window:

`firefox --new-window {{https://www.duckduckgo.com}}`

- Open a private (incognito) window:

`firefox --private-window`

- Search for "wikipedia" using the default search engine:

`firefox --search "{{wikipedia}}"`

- Launch Firefox in safe mode, with all extensions disabled:

`firefox --safe-mode`

- Take a screenshot of a web page in headless mode:

`firefox --headless --screenshot {{path/to/output_file.png}} {{https://example.com/}}`

- Use a specific profile to allow multiple separate instances of Firefox to run at once:

`firefox --profile {{path/to/directory}} {{https://example.com/}}`

- Set Firefox as the default browser:

`firefox --setDefaultBrowser`
