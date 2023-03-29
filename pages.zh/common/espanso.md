# espanso 
## chatgpt 
espanso 是一个开源的快捷文本扩展工具，可以帮助用户更快速地输入常用的短语、词组等内容。espanso 通过简单的命令行操作，将用户设置的文本扩展绑定到特定的快捷词汇上，从而实现快速输入。

使用命令 espanso，用户可以：

- 列出当前所有的扩展词汇列表
- 添加/删除扩展词汇
- 显示扩展词汇的详细信息
- 启动和停止 espanso 服务

例如，以下是一些常用的 espanso 命令：

- `espanso start`：启动 espanso 服务
- `espanso stop`：停止 espanso 服务
- `espanso list`：列出所有的扩展词汇列表
- `espanso edit`：编辑 espanso 配置文件
- `espanso add`：添加新的扩展词汇
- `espanso delete`：删除已有的扩展词汇
- `espanso version`：显示 espanso 的版本信息

在使用 espanso 前，用户需要先定义要扩展的内容和绑定的快捷词汇。具体细节可参考 espanso 官方文档。 

## tldr 
 
> 用 Rust 编写的跨平台文本扩展器。
> 更多信息：<https://espanso.org>.

- 检查状态：

`espanso status`

- 编辑配置：

`espanso edit config`

- 从 hub 商店（<https://hub.espanso.org/>）安装一个软件包：

`espanso install {{软件包的名字}}`

- 重新启动（安装软件包后需要，在失败的情况下很有用）：

`espanso restart`
