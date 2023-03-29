# virtualenv 
## chatgpt 
virtualenv是一个用于创建Python虚拟环境的工具。

虚拟环境是一个完全独立的Python运行环境，它包含自己的安装包、解释器、库和环境变量。使用虚拟环境，可以隔离不同项目所使用的Python包，避免不同版本之间的冲突。

使用virtualenv命令创建虚拟环境的步骤如下：

1. 安装virtualenv。

可以通过pip安装virtualenv：

```
$ pip install virtualenv
```

2. 创建虚拟环境。

创建虚拟环境的方式如下：

```
$ virtualenv [虚拟环境名称]
```

虚拟环境名称可以任意指定，比如：

```
$ virtualenv venv
```

这将在当前目录下创建一个名为“venv”的虚拟环境。

3. 激活虚拟环境。

创建虚拟环境后，需要激活虚拟环境才能使用它。

在Linux或Mac OS X上，可以使用以下命令激活虚拟环境：

```
$ source venv/bin/activate
```

在Windows上，可以使用以下命令激活虚拟环境：

```
$ venv\Scripts\activate
```

激活虚拟环境后，命令行提示符会发生改变，显示当前处于哪个虚拟环境中。

4. 使用虚拟环境。

激活虚拟环境后，可以使用pip安装依赖包，并进行Python开发。在虚拟环境中安装的依赖包和使用的Python版本，都不会影响系统范围内的Python环境。

5. 退出虚拟环境。

完成开发后，可以使用以下命令退出虚拟环境：

```
$ deactivate
```

退出虚拟环境后，命令行提示符会回到原来的样子。虚拟环境中安装的依赖包和使用的Python版本，都不再影响系统范围内的Python环境。 

## tldr 
 
> 创建被隔离的的 Python 虚拟环境。
> 更多信息：<https://virtualenv.pypa.io/>.

- 创建新环境：

`virtualenv {{path/to/venv}}`

- 自定义提示符：

`virtualenv --prompt={{prompt_prefix}} {{path/to/venv}}`

- 为虚拟环境使用不同的 Python 版本：

`virtualenv --python={{path/to/pythonbin}} {{path/to/venv}}`

- 启动（选择）环境：

`source {{path/to/venv}}/bin/activate`

- 停止环境：

`deactivate`
