# pyenv 
## chatgpt 
pyenv 是一种 Python 版本管理工具，它可以让您在同一台计算机上轻松安装和切换多个 Python 版本，以满足不同项目的要求。有了 pyenv，您可以在一个项目中使用 Python 2.7，而在另一个项目中使用 Python 3.6，而无需在计算机上安装多个 Python 版本。

pyenv 的主要命令包括：

1. pyenv install：安装指定版本的 Python，并自动配置环境变量。

2. pyenv versions：列出已安装的 Python 版本。

3. pyenv global：设置全局 Python 版本。

4. pyenv local：在当前目录下设置特定的 Python 版本。

5. pyenv virtualenv：创建和管理虚拟 Python 环境。

6. pyenv shell：在当前 shell 中设置特定的 Python 版本。

7. pyenv which：显示指定的命令或可执行文件使用哪个 Python 解释器。

8. pyenv whence：查找指定命令在哪个目录中可用。

总之，pyenv 可以使 Python 版本管理更加简单和灵活，为开发人员提供了更多的选择和自由，使他们能够更高效、便捷地进行开发工作。 

## tldr 
 
> 在多个 Python 版本之间轻松切换。
> 更多信息：<https://github.com/pyenv/pyenv>.

- 列出所有可用的命令：

`pyenv commands`

- 列出 `${PYENV_ROOT}/versions` 目录下的所有 Python 版本：

`pyenv versions`

- 列出所有可以从上游安装的 Python 版本：

`pyenv install --list`

- 在 `${PYENV_ROOT}/versions` 目录下安装一个 Python 版本：

`pyenv install {{2.7.10}}`

- 在 `${PYENV_ROOT}/versions` 目录下卸载一个 Python 版本：

`pyenv uninstall {{2.7.10}}`

- 设置在当前机器中全局使用的 Python 版本：

`pyenv global {{2.7.10}}`

- 设置在当前目录及其下所有目录中使用的 Python 版本：

`pyenv local {{2.7.10}}`
