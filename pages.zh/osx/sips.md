# sips 
## chatgpt 
`sips` 是 macOS 操作系统中的一个命令行工具，全称为 Scriptable Image Processing System，它用于处理图像文件。通过 `sips` 命令，用户可以使用命令行界面（CLI）对图像文件执行以下操作：

1. 缩放图片尺寸
2. 翻转、旋转、翻转和旋转图片
3. 转换图片格式
4. 添加图片描述信息
5. 裁剪图片
6. 调整图片方向
7. 替换图片色彩空间（比如 RGB、CMYK 等）
8. 批量处理图像。

下面是一些 `sips` 命令的示例：

1. 缩小图像尺寸：

`sips -Z 500 image.jpg`

该命令将 image.jpg 图像的宽度和高度缩小至 500 像素，但是该命令不会保持原始宽高比。

2. 转换图像格式：

`sips -s format png image.jpg --out newimage.png`

该命令将 image.jpg 转换为 png 格式的图像，新图像保存在 newimage.png 文件中。

3. 裁剪图像

`sips -c 50 50 250 250 image.jpg --out croppedImage.jpg`

该命令将 image.jpg 图像从左上角（50,50）开始裁剪，裁剪的大小是 250×250 像素，新图像保存在 croppedImage.jpg 文件中。

4. 调整图像方向

`sips -r 90 image.jpg --out rotatedImage.jpg`

该命令将 image.jpg 图像顺时针旋转 90 度，新图像保存在 rotatedImage.jpg 文件中。

总之，`sips` 是一款功能强大的命令行工具，能够方便快捷地处理图像文件，可用于各种自动化脚本、批量处理等场景。 

## tldr 
 
> 苹果的处理文件脚本系统。
> 光栅 / 查询图像 和 颜色同步 ICC 配置文件。
> 更多信息：<https://ss64.com/osx/sips.html>.

- S 指定一个输出目录，这样原始文件就不会被修改：

`sips --out {{目标 / 文件夹 / 输出文件夹}}`

- 以指定的大小对图像重新采样，图像纵横比可能会更改：

`sips -z {{1920}} {{300}} {{图片文件。扩展名}}`

- 对图像重新取样，使高度和宽度不大于指定的大小（注意大写 Z）：

`sips -Z {{1920}} {{300}} {{图片文件。扩展名}}`

- 对目录中的所有图像重新取样，以适应 960px 的宽度（保持纵横比）：

`sips --resampleWidth {{960}} {{目标 / 文件夹 / 所有图片文件}}`

- 将图像从 CMYK 转换为 RGB：

`sips --matchTo '/System/Library/ColorSync/Profiles/Generic RGB Profile.icc' {{目标 / 文件夹 / 图片。扩展}} {{目标 / 文件夹 / 输出文件夹}}`

- 从图像中删除 ColorSync ICC 配置：

`sips -d profile --deleteColorManagementProperties {{目标 / 文件夹 / 图片。扩展}}`
