# GetFileInfo 
## chatgpt 
GetFileInfo是macOS中的一个命令行工具，用于查看指定文件的元数据（metadata）。元数据指的是与文件相关的信息，如文件名、大小、创建时间、修改时间、所属用户、所属组等等。以下是该命令的详细用法：

语法：

GetFileInfo [-aafmprstux] [-d format] [-s suffix] [-c] [-h] [-q] [-v] file ...

参数：

-a：显示文件的所有元数据

-f：在输出中包括文件名

-m：在输出中包括文件类型与创造日期

-p：在输出中包括 POSIX 文件权限信息

-r：递归处理目录中所有文件和子目录

-s suffix：使用指定的后缀名来确定文件类型

-t：在输出中包括文件创建和修改时间

-u：在输出中包括用户和组信息

-x：在输出中包括扩展属性

-d format：在输出中按照指定的格式显示日期和时间，其中format可以是：

%a：星期的缩写（例如 Mon）
%A：星期的全称（例如 Monday）
%b：月份的缩写（例如 Jan）
%B：月份的全称（例如 January）
%c：按照系统本地日期和时间显示
%d：天数（例如，01~31）
%H：小时（24小时制）
%I：小时（12小时制）
%j：一年中的第几天（001~366）
%m：月份（01~12）
%M：分（00~59）
%p：AM或PM
%S：秒（00~60）
%U：%U是指在当年中第几周，周日被认定为每周的第一天
%w：星期几的数字表示，0代表星期天
%W：在当年中第几周，周一被认定为每周的第一天
%x：使用系统本地日期格式
%X：使用系统本地时间格式
%y：年份的最后两位数
%Y：年份

-c：在输出中不包括文件名，以便进行批处理

-h：文件名中如果包含空格，则使用双引号进行引用

-q：在输出中不包括额外的信息，只打印元数据

-v：打印 GetFileInfo 的版本信息

file：要查看元数据的文件路径

示例：

要查看文件sample.txt的所有元数据，可以使用以下命令：

GetFileInfo -a sample.txt

要查看文件sample.txt的创建和修改时间，可以使用以下命令：

GetFileInfo -t sample.txt

要查看文件sample.txt的文件类型和创建时间，可以使用以下命令：

GetFileInfo -m sample.txt

要查看文件sample.txt的文件名和文件大小，可以使用以下命令：

GetFileInfo -f -s byte sample.txt

要查看目录mydir下所有文件的元数据，可以使用以下命令：

GetFileInfo -r mydir

GetFileInfo命令可以帮助用户查看文件的元数据信息，方便用户了解文件的相关信息，在日常工作中广泛应用。 

## tldr 
 
> 获取有关 HFS+ 目录中文件的信息。
> 更多信息：<https://www.unix.com/man-page/osx/1/GetFileInfo/>.

- 显示有关给定文件的信息：

`GetFileInfo {{路径/文件名}}`

- 显示给定文件的创建日期和时间：

`GetFileInfo -d {{路径/文件名}}`

- 显示给定文件的上次修改日期和时间：

`GetFileInfo -m {{路径/文件名}}`

- 显示给定文件的创建者：

`GetFileInfo -c {{路径/文件名}}`
