# gcp 
## chatgpt 
`gcp` 是一个Linux/Unix下的命令，用于将文件或目录从一个位置复制到另一个位置。该命令的完整形式为 `gcp`（GNU Core Utilities），是GNU工具集中的一部分。

下面是 `gcp` 命令的常用选项和参数：

```bash
gcp [OPTIONS] SOURCE_FILE DESTINATION_DIRECTORY
```

### 选项

- `-r`：递归复制，复制目录及其所有子目录和文件。如果不指定此选项，仅复制单个文件。
- `-p`：同时复制文件属性，如权限、时间戳等。如果不指定此选项，则清空目标文件的原有属性。
- `-v`：显示文件复制过程。
- `-u`：仅在源文件比目标文件新或不存在时才复制（更新模式）。
- `-i`：在覆盖已存在的目标文件之前，提示用户确认处理。

### 示例

1. 将文件 `file1.txt` 复制到目录 `/home/user1/documents/`：

   ```bash
   gcp file1.txt /home/user1/documents/
   ```

2. 进行递归复制，将目录 `dir1` 和所有子目录中的文件复制到目录 `/home/user1/downloads/`：

   ```bash
   gcp -r dir1 /home/user1/downloads/
   ```

3. 使用 `-p` 选项，复制文件 `file1.txt` 到目录 `/home/user1/documents/`，同时保留原有文件属性：

   ```bash
   gcp -p file1.txt /home/user1/documents/
   ```

4. 运行交互模式，复制文件 `file1.txt` 到目录 `/home/user1/documents/` 之前提示用户确认处理：

   ```bash
   gcp -i file1.txt /home/user1/documents/
   ```

`gcp` 命令与其他类似的命令 `cp` 和 `mv` 功能类似，但是在某些方面，如递归复制和保留文件属性等方面有所不同。 

## tldr 
 
> 这是 `-p linux cp` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux cp`
