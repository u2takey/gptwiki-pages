# unflatten 
## chatgpt 
unflatten是一个用于转换扁平化后的输入数据的命令。具体来说，它将扁平化的输入数据转换为一个更易于理解和处理的格式。 

在具体使用中，unflatten主要有以下两个作用： 

1. 将扁平化数据还原成嵌套格式：在某些情况下，我们需要将嵌套的数据结构转换为扁平化格式。但当我们需要读取这些扁平化数据并转换回嵌套格式时，可以使用 unflatten 命令。 

2. 将XML或JSON数据转换为可读格式：假设我们有一个XML或JSON文件，但它的格式非常紊乱，不容易阅读。使用unflatten命令可以将其转换为易于阅读格式。 

另外，unflatten命令也可以通过使用不同的标志和选项来帮助用户控制其输出行为和格式。 

总的来说，unflatten是一个非常实用的命令，适用于各种不同情况下的数据转换和整理。 

## tldr 
 
> 调整有向图以改善布局的纵横比。
> Graphviz 过滤器: `acyclic`, `bcomps`, `comps`, `edgepaint`, `gvcolor`, `gvpack`, `mingle`, `nop`, `sccmap`, `tred`, 和 `unflatten`。
> 更多信息: <https://www.graphviz.org/pdf/unflatten.1.pdf>.

- 调整一个或多个有向图以改善布局的纵横比:

`unflatten {{路径/到/输入1.gv}} {{路径/到/输入2.gv ...}} > {{路径/到/输出.gv}}`

- 将 `unflatten` 作为 `dot` 布局的预处理器以改善纵横比:

`unflatten {{路径/到/输入.gv}} | dot -T {{png}} {{路径/到/输出.png}}`

- 显示 `unflatten` 的帮助:

`unflatten -?`
