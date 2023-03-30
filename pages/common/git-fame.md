# git fame 
## chatgpt 
Git Fame is not a built-in command in Git. Instead, it is a third-party tool that provides a visual representation of the project's contributors over time. 

Git Fame analyzes the Git repository and generates an interactive HTML page that shows a graph of contributors' activities. The graph displays the number of commits, lines added, and lines deleted by each contributor. 

It also provides a leaderboard that lists the most active contributors based on their commit activity. Additionally, it generates a timeline that provides a detailed view of the project's activity, showing the number of commits made each week by each author. 

To use Git Fame, you need to install the tool first. Usually, you can install it via the command: 

```
npm install -g git-fame
```

After installation, you can run `git fame` command in the terminal to generate the report. The output will be an interactive HTML page that you can open in a web browser.

Overall, Git Fame is a useful tool to visualize the contributions made by different developers to a project over time. 

## tldr 
 
> Pretty-print Git repository contributions.
> More information: <https://github.com/casperdcl/git-fame>.

- Calculate contributions for the current Git repository:

`git fame`

- Exclude files/directories that match the specified regular expression:

`git fame --excl "{{regular_expression}}"`

- Calculate contributions made after the specified date:

`git fame --since "{{3 weeks ago|2021-05-13}}"`

- Display contributions in the specified format:

`git fame --format {{pipe|yaml|json|csv|tsv}}`

- Display contributions per file extension:

`git fame --bytype`

- Ignore whitespace changes:

`git fame --ignore-whitespace`

- Detect inter-file line moves and copies:

`git fame -C`

- Detect intra-file line moves and copies:

`git fame -M`
