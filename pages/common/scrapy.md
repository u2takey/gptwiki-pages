# scrapy 
## chatgpt 
Scrapy is a Python-based web crawling framework used for extracting data from websites. It is an open source tool that allows you to scrape data from a website with ease. The basic command to run Scrapy is "scrapy", and it is followed by various options and arguments.

Here is a breakdown of the "scrapy" command and its various options and arguments:

1. scrapy startproject: This command is used to create a new Scrapy project. You need to provide a project name after this command, for example, "scrapy startproject myproject".

2. scrapy crawl: This command is used to run a spider (a program that crawls a website and extracts data) that you have defined in your Scrapy project. You need to provide a spider name after this command, for example, "scrapy crawl myspider".

3. scrapy list: This command will list all the spiders that are available in your Scrapy project. You can use this command to verify if your spider is installed properly.

4. scrapy shell: This command opens up an interactive shell where you can test your spider and run commands to extract data from a website.

5. scrapy genspider: This command is used to generate a new spider. You need to provide a spider name and the website URL you want to crawl, for example, "scrapy genspider myspider mywebsite.com".

6. scrapy deploy: This command is used to deploy your Scrapy project to a remote server. It requires some additional configuration, including an authentication token and the remote server URL.

These are some of the basic commands that you can run with Scrapy. However, there are many other options and arguments available that you can explore for your specific use case. 

## tldr 
 
> Web-crawling framework.
> More information: <https://scrapy.org>.

- Create a project:

`scrapy startproject {{project_name}}`

- Create a spider (in project directory):

`scrapy genspider {{spider_name}} {{website_domain}}`

- Edit spider (in project directory):

`scrapy edit {{spider_name}}`

- Run spider (in project directory):

`scrapy crawl {{spider_name}}`

- Fetch a webpage as Scrapy sees it and print the source to `stdout`:

`scrapy fetch {{url}}`

- Open a webpage in the default browser as Scrapy sees it (disable JavaScript for extra fidelity):

`scrapy view {{url}}`

- Open Scrapy shell for URL, which allows interaction with the page source in a Python shell (or IPython if available):

`scrapy shell {{url}}`
