# resume 
## chatgpt 
The "resume" command is usually used to continue the execution of a previously suspended job or process in a Unix-like operating system. It's typically used after the "suspend" command, which temporarily stops a background job, process or task.

When you type "resume" followed by the job or process ID, the operating system will resume the job from the point where it was suspended, allowing it to continue running in the background.

For example, if you had previously suspended a long-running process with the ID of 1234 using the "suspend" command, you can resume it using the "resume" command like this:

```
resume 1234
```

Once the command is executed, the process will continue running in the background, and you regain control of the terminal prompt, allowing you to continue working on other tasks.

It's worth noting that the "resume" command may not work in all cases, and it will only work for jobs or processes that have been previously suspended. If the process has already finished or is currently running in the foreground, the "resume" command will have no effect. 

## tldr 
 
> CLI tool to easily setup a new resume.
> More information: <https://github.com/jsonresume/resume-cli>.

- Create a new `resume.json` file in the current working directory:

`resume init`

- Validate a `resume.json` against schema tests to ensure it complies with the standard:

`resume validate`

- Export a resume locally in a stylized HTML or PDF format:

`resume export {{path/to/html_or_pdf}}`

- Start a web server that serves a local `resume.json`:

`resume serve`
