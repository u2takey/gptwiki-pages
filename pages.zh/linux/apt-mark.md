# apt-mark 
## chatgpt 
apt-mark是Linux系统中的一个命令，它主要用于管理APT软件包管理器中的各种标记信息。以下是apt-mark命令的详细解释：

1. apt-mark showauto：显示自动安装的软件包列表。

2. apt-mark showmanual：显示手动安装的软件包列表。

3. apt-mark showhold：显示设置为hold状态的软件包列表。

4. apt-mark showall：显示所有软件包列表。

5. apt-mark unmarkauto：取消自动安装的软件包标记。

6. apt-mark unmarkmanual：取消手动安装的软件包标记。

7. apt-mark unmarkhold：取消设置为hold状态的软件包标记。

8. apt-mark auto：将软件包设置为自动安装。

9. apt-mark manual：将软件包设置为手动安装。

10. apt-mark hold：将软件包设置为“hold”状态，停止其更新。 

## tldr 
 
> 修改已安装软件包状态的工具。
> 更多信息：<https://manpages.debian.org/latest/apt/apt-mark.8.html>.

- 将一个软件包标记为自动安装：

`sudo apt-mark auto {{软件包名}}`

- 将一个软件包保持在当前版本，防止对其更新：

`sudo apt-mark hold {{软件包名}}`

- 允许对一个软件包更新：

`sudo apt-mark unhold {{软件包名}}`

- 列出手动安装的软件包：

`apt-mark showmanual`

- 列出保持当前版本而不更新的软件包：

`apt-mark showhold`
