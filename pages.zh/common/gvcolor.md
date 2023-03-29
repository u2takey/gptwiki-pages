# gvcolor 
## chatgpt 
gvcolor是Graphviz软件包中的一个命令行工具，用于为图形设置颜色。它可以根据给定的颜色方案或算法为图形中的节点和边缘分配颜色。

使用gvcolor命令，可以生成一组颜色方案以配合特定的图形，或者使用现有的颜色方案。该命令支持多种颜色分配算法，包括均匀分布、负载均衡和随机分配。

要使用gvcolor设置颜色，需要指定输入的图形文件和一个颜色方案。例如，下面的命令将为文件input.dot中的节点和边缘创建一个色彩方案，并将结果输出到output.dot文件中：

```
gvcolor -o output.dot input.dot
```

此外，gvcolor还支持通过指定颜色标记覆盖默认的颜色选择方案。

总之，gvcolor命令是Graphviz工具包中一个强大的工具，可用于为图形元素分配颜色，以帮助用户更好地理解和解释图形数据。 

## tldr 
 
> 用一系列颜色为有序有向图着色。
> Graphviz 过滤器: `acyclic`, `bcomps`, `comps`, `edgepaint`, `gvcolor`, `gvpack`, `mingle`, `nop`, `sccmap`, `tred`, & `unflatten`。
> 更多信息: <https://graphviz.org/pdf/gvcolor.1.pdf>.

- 为一个或多个已被 `dot` 处理的有序有向图着色:

`gvcolor {{路径/到/布局1.gv}} {{路径/到/布局2.gv ...}} > {{路径/到/输出.gv}}`

- 对一个图进行布局和着色，然后将其转换为 PNG 图像:

`dot {{路径/到/输入.gv}} | gvcolor | dot -T {{png}} > {{路径/到/输出.png}}`

- 显示 `gvcolor` 的帮助信息:

`gvcolor -?`
