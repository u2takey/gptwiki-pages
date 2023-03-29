# bg 
## chatgpt 
命令：bg

作用：将一个已停止的作业转入后台运行

解释：

bg命令用于将一个已经停止（即被挂起）的作业转入后台运行，使终端可以返回到命令行提示符。

一般情况下，作业会在前台运行，当用户按下CTRL+Z组合键时，作业将会停止（挂起），并返回到命令行提示符处。此时可以使用bg命令将作业转入后台继续运行。

使用方式：bg [JOB ID]

其中，JOB ID是指需要转入后台运行的作业的ID号。

示例：

假设用户在前台运行了一个长时间的命令，比如：

$ python3 mylongrunning_script.py

然后按下CTRL+Z将命令挂起。

此时可以使用jobs命令查看当前已有的作业，并找到对应的作业ID：

$ jobs
[1]+  Stopped                 python3 mylongrunning_script.py

可以看到，ID为1的作业被挂起。

使用bg命令将该作业转入后台运行：

$ bg 1
[1]+ python3 mylongrunning_script.py &

可以看到，作业已经被转入后台运行，并在末尾加上了“&”符号。

接下来，用户可以继续在终端进行其他操作，该作业会在后台默默地继续执行。

注意事项：

1. 如果不指定JOB ID，则默认将最近一个被挂起的作业转入后台运行。

2. 转入后台运行的作业仍然会在终端输出信息，但是输出信息不会直接显示在当前终端窗口，而是被重定向到后台进程，可以使用jobs命令查看这些作业的运行结果。如果需要实时查看转入后台运行的作业的输出信息，可以使用命令tail -f在另一个终端窗口中跟踪输出日志。 

## tldr 
 
> 恢复被挂起的任务（如. 使用 Ctrl + Z），使它们在后台运行。
> 更多信息：<https://manned.org/bg>.

- 恢复最近被挂起的任务，在后台运行：

`bg`

- 恢复特定的任务（使用 `jobs -l` 可以获取任务 ID）并在后台运行：

`bg %{{job_id}}`