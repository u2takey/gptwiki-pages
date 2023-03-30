# duti 
## chatgpt 
duti是一种命令行实用工具，用于设置默认应用程序和文件类型处理器。duti的语法如下：

```
duti [-s] [-u] [-x extension [bundle_id]] [-a app_id [bundle_id]] [-d extension] [-e] [-h] [filename]
```

参数解释：

- -s：显示当前设置的默认应用程序和文件类型处理器；
- -u：重置所有默认应用程序和文件类型处理器；
- -x：指定文件后缀名，后跟所需的工具包标识符（可选参数）。删除此组合可删除文件后缀名的关联；
- -a：指定应用程序标识符和（可选）此应用程序应用的包标识符。删除此组合将删除应用程序/包的关联；
- -d：删除文件扩展名或类型的关联；
- -e：显示所有可执行文件和它们的信息，包括应用程序标识符、应用程序名称和应用程序所需的包标识符；
- -h：显示duti的帮助文件。

使用duti可以让用户定制他们的工作流程更加高效，使得在打开文件时可以自动使用指定的程序进行处理，从而更加智能化、自动化、高效化等等。 

## tldr 
 
> 在 macOS 上为文档类型和网页设置默认打开的应用程序。
> 更多信息：<https://github.com/moretension/duti>.

- 将 Safari 设置为 HTML 文档的默认打开程序：

`duti -s {{com.apple.Safari}} {{public.html}} all`

- 将 vlc 设置为扩展名为.m4v 的文件的默认查看器：

`duti -s {{org.videolan.vlc}} {{m4v}} viewer`

- 将 Finder 设置为 ftp:// URL 访问的应用：

`duti -s {{com.apple.Finder}} {{ftp}}`

- 显示有关给定扩展名的默认应用程序的信息：

`duti -x {{ext}}`

- 显示给定的 UTI 对应默认的处理程序：

`duti -d {{uti}}`

- 显示给定 UTI 对应所有的处理程序：

`duti -l {{uti}}`
