# color 
## chatgpt 
命令 `color` 用于更改在 Windows 命令提示符中使用的前景（文字）和背景颜色。以下是该命令的详细信息：

语法：
```
color [colorvalue]
```

参数：
* `colorvalue`：可选参数，指定要使用的新颜色值。此值应为 0 到 f（16 进制值），其中每个值对应一种颜色组合。

适用的版本：
* 适用于所有 Windows 版本。

示例：
* 要更改前景色为绿色，背景色为红色，可以在命令提示符下键入：`color 4a`。其中，“4”是红色的值，而“a”是绿色的值。您也可以使用其他颜色值组合。

注意事项：
* 如果未指定任何参数，则将显示当前颜色的值。
* 若要永久更改默认颜色，请更改命令提示符的属性。 

## tldr 
 
> 设置控制台的前景色和背景色。
> 更多信息：<https://learn.microsoft.com/windows-server/administration/windows-commands/color>.

- 将控制台颜色恢复至默认值：

`color`

- 列出可用的颜色值和详细信息：

`color /?`

- 将控制台前景色和背景色设置为指定颜色：

`color {{前景色值}}{{背景色值}}`