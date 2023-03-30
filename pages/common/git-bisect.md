# git bisect 
## chatgpt 
The `git bisect` command is used to perform a binary search through the commit history of a Git repository. It is used primarily to find a specific commit that introduced a bug or a regression. 

To use `git bisect`, you begin by identifying a "known good" commit, that is a commit in which the code was working correctly, and a "known bad" commit, that is a commit in which the bug or regression was present. 

You then run the command `git bisect start`, which will put Git in bisect mode. 

Next, you specify the "known good" and "known bad" commits by running the commands `git bisect good <good-commit>` and `git bisect bad <bad-commit>`.

Git will then checkout a commit that is the midway between the two commits (the "middle" commit) and it's up to you to test this commit to see whether the issue is present or not. 

Based on the result of the test, you will then run either `git bisect good` or `git bisect bad`:
- `git bisect good` if the middle commit is working as expected
- `git bisect bad` if the middle commit has the issue you're attempting to troubleshoot

As you continue to run these `git bisect` commands, it will gradually narrow down to a small set of commits that are likely to be the ones that introduced the issue. At that point, you can examine those remaining commits more closely to identify the specific commit that is responsible for the issue.

Once you have found the culprit commit, you can use Git's usual tools to fix the problem, such as reverting the commit or creating a new one that resolves the issue. Finally, you exit bisect mode by running the command `git bisect reset`. 

## tldr 
 
> Use binary search to find the commit that introduced a bug.
> Git automatically jumps back and forth in the commit graph to progressively narrow down the faulty commit.
> More information: <https://git-scm.com/docs/git-bisect>.

- Start a bisect session on a commit range bounded by a known buggy commit, and a known clean (typically older) one:

`git bisect start {{bad_commit}} {{good_commit}}`

- For each commit that `git bisect` selects, mark it as "bad" or "good" after testing it for the issue:

`git bisect {{good|bad}}`

- After `git bisect` pinpoints the faulty commit, end the bisect session and return to the previous branch:

`git bisect reset`

- Skip a commit during a bisect (e.g. one that fails the tests due to a different issue):

`git bisect skip`

- Display a log of what has been done so far:

`git bisect log`
