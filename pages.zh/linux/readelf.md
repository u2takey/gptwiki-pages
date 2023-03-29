# readelf 
## chatgpt 
readelf 是一个用于查看ELF (Executable and Linkable Format) 格式可执行文件，目标文件，共享目标文件和 core dump 文件的命令行工具。它可以解析出二进制文件的各种节（section），包括符号表、节头、程序头、动态节等，并输出它们的详细信息。

readelf 命令一般用于以下方面：

1. 查找二进制文件的各种节信息

以下是 readelf 命令常用的选项：

- -a 或 -A：显示所有信息（包括头信息）。
- -h 或 --file-header：显示文件头信息。
- -S 或 --sections：显示所有节的名称和地址。
- -s 或 --symbols：显示所有符号（全局变量或函数）的名称和地址。
- -d 或 --dynamic：显示动态节的名称和内容。
- -x <sectionName> 或 --hex-dump=<sectionName>：以十六进制格式显示指定节的内容。

例如，要查看一个可执行文件的所有节信息，可以在终端中输入以下命令：

```
readelf -a executable_file
```

2. 查找符号表

符号表是记录了程序中变量、函数名称及其地址等信息的表，通常用于调试和动态链接。readelf 命令可以输出所有符号表中的信息，包括名称、地址、符号类型等。

下面是输出符号表信息的命令：

```
readelf -s executable_file
```

3. 查找动态链接相关信息

readelf 命令可以输出动态链接的相关信息，包括动态链接库名称、符号解析表等，这对于调试和了解程序的动态链接信息非常有用。

下面是输出动态链接信息的命令：

```
readelf -d executable_file
```

总的来说，readelf 命令是一个非常实用的工具，它可以帮助我们深入理解二进制文件的内部结构和细节。因此，在平时的程序开发和调试中，使用 readelf 命令可以提高我们的工作效率和质量。 

## tldr 
 
> 显示 EFI 文件信息。
> 更多信息：<http://man7.org/linux/man-pages/man1/readelf.1.html>.

- 显示 ELF 所有文件信息：

`readelf -all {{path/to/binary}}`

- 显示 ELF 文件的所有头信息：

`readelf --headers {{path/to/binary}}`

- 如果存在符号表项，则显示 ELF 文件内的符号表项：

`readelf --symbols {{path/to/binary}}`

- 显示 ELF 文件头信息：

`readelf --file-header {{path/to/binary}}`
