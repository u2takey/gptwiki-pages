# exit 
## chatgpt 
exit命令是用来退出正在运行的命令行终端窗口或退出当前正在运行的脚本程序。该命令根据情况可能会给出一个退出状态码（exit code），表示上一个命令成功执行（exit code为 0），或者由于某种原因无法执行（exit code为大于 0 的值）。

在命令行中，当我们键入exit命令并按下回车键时，会直接关闭当前的终端窗口。如果我们在某个脚本程序中编写了exit命令，当脚本程序执行到该命令时，程序将会停止执行，并退出程序。还有一种情况是，如果我们在命令行中使用exit n命令，那么它将会退出当前的终端窗口，并返回一个值为n的exit code。

需要注意的是，在使用exit命令退出终端窗口时，我们需要确保自己保存好所有需要保存的文件。因为一旦退出了终端窗口，所有未保存的工作都将会丢失。 

## tldr 
 
> 退出终端程序。
> 更多信息：<https://manned.org/exit>.

- 使用最后执行命令的退出代码，退出终端程序：

`exit`

- 使用指定的退出代码，退出终端程序：

`exit {{exit_code}}`