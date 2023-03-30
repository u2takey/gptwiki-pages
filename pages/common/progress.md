# progress 
## chatgpt 
As an AI language model, I do not have sufficient information to accurately respond to your question. Can you please provide more context or specify which command you are referring to? 

## tldr 
 
> Display/Monitor the progress of running coreutils.
> More information: <https://github.com/Xfennec/progress>.

- Show the progress of running coreutils:

`progress`

- Show the progress of running coreutils in quiet mode:

`progress -q`

- Launch and monitor a single long-running command:

`{{command}} & progress --monitor --pid $!`

- Include an estimate of time remaining for completion:

`progress --wait --command {{firefox}}`
