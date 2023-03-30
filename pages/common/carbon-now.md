# carbon-now 
## chatgpt 
As an AI language model, I cannot execute commands, but I can explain to you what "carbon-now" is and what it does.

Carbon-Now is an open-source command-line tool that helps you generate beautiful and customizable images of your code snippets with proper syntax highlighting, the ability to choose fonts, themes, and over 200 presets. These images are called "carbonized code snippets". Carbon-Now is especially helpful when you want to share code snippets on social media, blogs, and other online platforms as it beautifies them and makes them more visually appealing.

When you run the "carbon-now" command in your terminal, it will ask you for the code snippet you want to carbonize. Then, it will open a browser window with the carbon.now.sh website loaded and display the carbonized code snippet. You can customize the snippet by changing the font, theme, background color, and other options before you generate the final image. The final image can be saved in PNG, JPEG or SVG formats. Carbon-Now also allows you to copy the code snippet as HTML and Markdown. 

Overall, Carbon-Now is a handy tool for developers who want to create visually appealing and customizable code snippets to share online. 

## tldr 
 
> Create beautiful images of code.
> More information: <https://github.com/mixn/carbon-now-cli>.

- Create an image from a file using default settings:

`carbon-now {{path/to/file}}`

- Create an image from a text in clipboard using default settings:

`carbon-now --from-clipboard`

- Create an image from standard input using default settings:

`{{input}} | carbon-now`

- Create images interactively for custom settings and optionally save a preset:

`carbon-now -i {{path/to/file}}`

- Create images from previously saved preset:

`carbon-now -p {{preset}} {{path/to/file}}`

- Start at a specified line of text:

`carbon-now -s {{line}} {{path/to/file}}`

- End at a specific line of text:

`carbon-now -e {{line}} {{path/to/file}}`

- Open image in a browser instead of saving:

`carbon-now --open {{path/to/file}}`
