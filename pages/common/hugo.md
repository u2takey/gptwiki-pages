# hugo 
## chatgpt 
Hugo is a static site generator which helps in creating websites. When the command "hugo" is executed, it generates a new static website or updates an existing one, depending on whether the user is creating a new site or updating an existing one.

Here are the steps taken by Hugo when the "hugo" command is executed:

1. Hugo scans the content directory of the website and converts the content (written in markdown or HTML) into HTML pages.

2. It then parses the website's configuration file (config.toml, config.yaml or config.json) to obtain site-wide settings such as theme, language, and other meta-data.

3. Hugo then builds the website and generates a static HTML file for each page, post or section of the website.

4. It also automatically generates an index file for each section, archive pages for posts, and a sitemap.xml file which makes it easier for search engines to index the website.

The "hugo" command is typically used in the terminal (or command prompt) after navigating into the folder that contains the website files. Once executed, the static files are generated in a directory named "public" (by default) within the root directory of the website. The user can then upload the files to a web server to make the website live. 

## tldr 
 
> Template-based static site generator. Uses modules, components, and themes.
> More information: <https://gohugo.io>.

- Create a new Hugo site:

`hugo new site {{path/to/site}}`

- Create a new Hugo theme (themes may also be downloaded from https://themes.gohugo.io/):

`hugo new theme {{theme_name}}`

- Create a new page:

`hugo new {{section_name}}/{{path/to/file}}`

- Build a site to the `./public/` directory:

`hugo`

- Build a site including pages that are marked as a "draft":

`hugo --buildDrafts`

- Build a site to a given directory:

`hugo --destination {{path/to/destination}}`

- Build a site, start up a webserver to serve it, and automatically reload when pages are edited:

`hugo server`
