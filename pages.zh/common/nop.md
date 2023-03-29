# nop 
## chatgpt 
指令nop是一个汇编指令，用于在程序执行期间暂时停止CPU的操作，但不会对寄存器或存储设备造成任何变化。nop指令通常是用作填充指令，以对齐内存地址或调整程序计数器（PC）值。nop指令的实现方式因处理器架构而异，但在大多数架构中，nop指令会简单地将CPU浪费的周期数增加一次。因此，当程序需要暂停一段时间以等待某些事件发生时，可以使用nop指令。 

## tldr 
 
> 检查有效性并以规范的格式漂亮地打印图形。
> Graphviz 过滤器：`acyclic`、`bcomps`、`comps`、`edgepaint`、`gvcolor`、`gvpack`、`mingle`、`nop`、`sccmap`、`tred` 和 `unflatten`。
> 更多信息： <https://www.graphviz.org/pdf/nop.1.pdf>.

- 漂亮地打印一个或多个规范格式的图形：

`nop {{路径/到/输入1.gv}} {{路径/到/输入2.gv ...}} > {{路径/到/输出.gv}}`

- 检查一个或多个图形的有效性，不生成输出图形：

`nop -p {{路径/到/输入1.gv}} {{路径/到/输入2.gv ...}}`

- 显示 `nop` 的帮助信息：

`nop -?`
