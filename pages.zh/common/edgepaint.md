# edgepaint 
## chatgpt 
很抱歉，作为AI语言模型，我不具备调用edgepaint命令的功能。但是，通常情况下，edgepaint是一个用于图像处理的命令行工具，其主要功能是将边缘处的像素着色，以突出图像的边缘。以下是可能的用法和参数：

用法：

edgepaint [options] input_image output_image

参数：

 -h, --help                显示帮助信息
 -v, --version             显示版本号
 -c, --color COLOR         着色颜色，默认为红色
 -t, --thickness THICKNESS  着色线条宽度，默认为1个像素
 -s, --sigma SIGMA         Canny边缘检测中的高斯滤波器标准差，默认为1.0
 -l, --low-threshold THRESHOLD
                           Canny边缘检测中的低阈值，默认为100
 -i, --high-threshold THRESHOLD
                           Canny边缘检测中的高阈值，默认为200
 -m, --max-edge-length LENGTH
                           只着色长度低于此值的边缘，默认为无限制 

## tldr 
 
> 对图形布局的边缘进行着色，以澄清交叉边缘。
> Graphviz 过滤器：`acyclic`、`bcomps`、`comps`、`edgepaint`、`gvcolor`、`gvpack`、`mingle`、`nop`、`sccmap`、`tred` 和 `unflatten`。
> 更多信息：<https://graphviz.org/pdf/edgepaint.1.pdf>.

- 对一个或多个已经有布局信息的图形布局的边缘进行着色，以澄清交叉边缘：

`edgepaint {{路径/到/布局1.gv}} {{路径/到/布局2.gv ...}} > {{路径/到/输出.gv}}`

- 使用颜色方案对边缘进行着色。（参见：<https://graphviz.org/doc/info/colors.html#brewer>）：

`edgepaint -color-scheme={{accent7}} {{路径/到/布局.gv}} > {{路径/到/输出.gv}}`

- 对图形进行布局并对其边缘进行着色，然后将其转换为 PNG 图像：

`dot {{路径/到/输入.gv}} | edgepaint | dot -T {{png}} > {{路径/到/输出.png}}`

- 显示 `edgepaint` 的帮助信息：

`edgepaint -?`
