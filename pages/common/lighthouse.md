# lighthouse 
## chatgpt 
Lighthouse is a command-line tool and an open-source project maintained by Google that helps developers improve the quality of their web pages. When you run the "lighthouse" command, it audits the web page in question against a set of best practices and guidelines, covering key categories such as performance, accessibility, and search engine optimization (SEO).

In more detail, the lighthouse command will perform the following actions:

1. Launch a headless Chrome browser instance to load the specified URL.
2. Simulate a slow network connection and a low-end mobile device to test the page's performance on different devices and networks.
3. Analyze the page's HTML, CSS, JavaScript, and other assets to identify potential issues that may impact user experience.
4. Generate a report that includes a score for each category, highlighting areas that need improvement and providing actionable tips and advice on how to fix them.

Some examples of the issues that Lighthouse may identify include:

- Large images that take a long time to load, causing a slow page speed.
- Accessibility issues, such as missing alternative text for images or improper use of headings.
- Inefficient use of JavaScript that slows down the page.
- Lack of HTTPS support, which can impact search engine rankings.
- Poor contrast ratios and color schemes that make it difficult for users to read the text.

The lighthouse command is used by developers, web designers, and content editors to ensure that their websites are optimized for performance, accessibility, and user experience. Additionally, Lighthouse can be integrated into automated testing pipelines and continuous integration processes to catch issues early on and ensure that any new changes do not negatively impact site quality. 

## tldr 
 
> Analyzes web applications and web pages, collecting modern performance metrics and insights on developer best practices.
> More information: <https://github.com/GoogleChrome/lighthouse>.

- Generate an HTML report for a specific website and save it to a file in the current directory:

`lighthouse {{https://example.com}}`

- Generate a JSON report and print it:

`lighthouse --output {{json}} {{https://example.com}}`

- Generate a JSON report and save it to a specific file:

`lighthouse --output {{json}} --output-path {{path/to/file.json}} {{https://example.com}}`

- Generate a report using the browser in headless mode without logging to `stdout`:

`lighthouse --quiet --chrome-flags="{{--headless}}" {{https://example.com}}`

- Generate a report, using the HTTP header key/value pairs in the specified JSON file for all requests:

`lighthouse --extra-headers={{path/to/file.json}} {{https://example.com}}`

- Generate a report for specific categories only:

`lighthouse --only-categories={{performance,accessibility,best-practices,seo,pwa}} {{https://example.com}}`

- Generate a report with device emulation and all throttling disabled:

`lighthouse --screenEmulation.disabled --throttling-method={{provided}} --no-emulatedUserAgent {{https://example.com}}`

- Display help:

`lighthouse --help`
