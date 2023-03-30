# xsltproc 
## chatgpt 
xsltproc是一个命令行工具，用于执行XSLT转换。

XSLT（Extensible Stylesheet Language Transformations）是一种基于XML的转换语言，可用于将一个XML文档转换成另一个XML文档或其他格式，比如HTML、文本文件等。xsltproc命令可用于执行XSLT转换的过程，将XML文档作为输入，同时提供一个XSL样式表来指定如何进行转换。

xsltproc命令支持多种选项，包括：

- -o：指定转换输出的文件名；
- --noout：不将结果输出到文件中，而是输出到标准输出中；
- --param：设置XSLT样式表的参数；
- --stringparam：在输入命令行上指定字符串参数；
- --output：指定输出格式（XML、HTML、文本等）。

xsltproc命令的具体用法如下所示：

xsltproc [选项] XSL-FILE XML-FILE

其中，XSL-FILE是XSLT样式表文件名，XML-FILE是输入的XML文件名。 

## tldr 
 
> 用 XSLT 转换 XML 以生成输出（通常是 HTML 或 XML）。
> 更多信息：<http://www.xmlsoft.org/xslt/xsltproc.html>.

- 使用特定的 XSLT 样式表转换 XML 文件：

`xsltproc --output {{输出.html}} {{样式表.xslt}} {{xml 文件.xml}}`

- 将值传递给样式表中的参数：

`xsltproc --output {{输出.html}} --stringparam {{键名}} {{值}} {{样式表.xslt}} {{xml 文件.xml}}`
