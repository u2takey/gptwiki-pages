# nativefier 
## chatgpt 
Nativefier is a command-line tool that allows you to package any web application or website into a standalone desktop application for Windows, Linux or macOS. 

The syntax of the nativefier command is:

`nativefier [options] <url> [dest]`

- `[options]`: These are custom options that you can set depending on your needs. Examples of options include specifying the name and icon of the application, setting the window size and position, specifying the platform you want to build the application for, and many others.
  
- `<url>`: This is the web application or website you want to package into a desktop application. It can be a fully functioning web app, a product or service, or even a marketing website.
  
- `[dest]`: This is optional and represents the directory where the generated app files will be saved.

Here's a step-by-step example of using the `nativefier` command to package a web application into a desktop application:

1. Open your terminal or command prompt and navigate to a directory where you want to save the generated app files (if you don't specify `[dest]`).
2. Type `nativefier <url>` and replace `<url>` with the web application or website you want to package into a desktop app.
3. If you want to set any custom options, you can add them after the URL. For example, `--name "My App"` will set the name of the generated app to "My App",`--icon path/to/icon.png` will set the icon for the app to the specified file.
4. Hit enter and wait for the nativefier tool to download and package the web application into a standalone desktop application.
5. Once the process completes, you will find the generated app in the specified `[dest]` directory (if you specified it) or in the current working directory. 

In summary, the `nativefier` command is a powerful tool for turning web applications or websites into standalone desktop applications with custom options and settings. 

## tldr 
 
> Command-line tool to create a desktop app for any web site with minimal configuration.
> More information: <https://github.com/jiahaog/nativefier>.

- Make a desktop app for a website:

`nativefier {{url}}`

- Create a desktop app with a custom name:

`nativefier --name {{name}} {{url}}`

- Use a custom icon, should be a PNG:

`nativefier --icon {{path/to/icon.png}} {{url}}`
